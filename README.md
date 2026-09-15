# SceneCap 0913

How a 103-second walk through an underground car park, recorded with a 360 camera and two GoPros, becomes
person-free vehicle-lens video with a metric range map behind every frame.

Open **https://zb8c5ek.github.io/scenecap-0913/** — the front page links to the four pages behind it:

| page | answers |
|---|---|
| `pipeline.html` | How does a walk through a garage become training clips? |
| `model.html` | Is the model itself any good? |
| `lens.html` | What does a delivered lens actually look like? |
| `status.html` | Where does production stand, and what did it cost? |

Every figure on these pages is read from the tools' own output at build time; none is typed by hand. The pages are
built by `pr_index_page.py`, `pr_flow_page.py`, `pr_results_page.py`, `pd_report.py` and `pd_status_page.py` in the
working repository, which is private - this repository holds only the rendered result.

Three caveats travel with the numbers: the metric scale is provisional (it follows from reading the painted bay
pitch as 2.5 m), the mesh carries one crater in the floor about two metres across, and the clip models declare
OPENCV_FISHEYE, whose reference implementation cannot evaluate the outer sixth of a 206-degree lens.
