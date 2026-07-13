# Week 1 — Getting Started with GIS
### GISS/GEOG 361/363 · Introduction to Geographic Information Science · Practice Lab

**Notebook:** `Week1_Getting_Started_with_GIS.ipynb`
**Status:** Practice lab — ungraded (see the Week 1 row of the Proposed Course Schedule)
**Region:** Silver City, Grant County, and the Gila National Forest, southwestern New Mexico

---

## Overview

This is the first lab of the semester. It's deliberately low-stakes: rather than teaching a GIS skill, it gets students oriented in **three parallel GIS platforms** — GeoLibre (web), QGIS (open-source desktop), and ArcGIS Pro (proprietary desktop) — using our home region, southwestern New Mexico, as a shared "practice place" before students choose their own place for the semester-long Place-Based Geospatial Inquiry Project in Week 2.

It also introduces the **Geo-Inquiry Process** (Ask → Collect → Visualize → Create → Act), the five-step structure every subsequent lab in this course follows.

## Learning Objectives

| Code | Outcome |
|---|---|
| K01 | GIS rests on a stable set of core concepts, expressed equivalently across proprietary and open-source tools. |
| S01 | Symbolizing and managing spatial data across layers (a first, gentle pass). |
| S10 | Evaluating and choosing between open-source and proprietary tools based on task, access, and sustainability. |
| A01 | Feeling confident and adaptable using both open-source and proprietary geospatial tools. |
| EQ1 (previewed) | What does this technology let us do, where are its limits, and who is excluded when using it costs money? |

## The Geo-Inquiry Process

This course structures every lab around the same five-step framework, adapted from National Geographic Education's Geo-Inquiry Process:

1. **Ask** — pose the question(s) driving the lab
2. **Collect** — get oriented and gather the needed data
3. **Visualize** — explore and look critically at what you've collected
4. **Create** — produce something (a map, a layer, an analysis)
5. **Act** — share, reflect, and connect it back to the driving question

Week 1 walks through all five steps at the lightest possible weight — the "data" is a basemap, and the "creation" is a single labeled point — so students get comfortable with the rhythm before the stakes rise.

## Platform Options

The notebook presents each step as three parallel, collapsible panels (`<details>` sections — they render as expandable "tabs" in Jupyter, JupyterLab, GitHub's notebook preview, and nbviewer). Students work through whichever platform(s) they're using.

### 🌐 GeoLibre (Web)
- **What it is:** A free, open-source, browser-based GIS (also available as a desktop/mobile app), built by Qiusheng Wu / opengeos. No account or install required.
- **Live app:** https://web.geolibre.app/ (also mirrored at https://viewer.geolibre.app/)
- **Docs & tutorials:** https://geolibre.app/
- **Why it's here:** it gives every student — regardless of machine, OS, or license access — a working GIS in under a minute, which is the whole point of the course's "parallel pathways, not primary + optional" framing.

### 🗺️ QGIS (Desktop, Open-Source)
- **Download:** https://qgis.org/download/
- Works on Windows, Mac, and Linux — this is the pathway for students without ArcGIS/Windows access.

### 💼 ArcGIS Pro (Desktop, Proprietary)
- Windows only; provided through the WNMU institutional license.
- Access instructions (install package, campus lab, or virtual desktop) should be posted as a Week 1 LMS announcement — link it in the notebook's setup section once finalized.

## Running the Notebook

- **No local GIS software required.** The notebook itself only needs a Jupyter environment (JupyterLab, classic Notebook, VS Code, Colab, or a JupyterHub instance) and, optionally, the `leafmap` package for two small preview cells.
- **Minimal install:**
  ```bash
  pip install leafmap
  ```
- **Hosted options:** if this notebook is published to a course GitHub repo, add Colab / Binder badges to the top cell (the same pattern used in the [EarthInquiryLab](https://github.com/asivitskis/EarthInquiryLab) demonstration lessons this course's lab format is modeled on).
- The embedded GeoLibre `IFrame` cell is optional and may not render in every hosted notebook environment (some block embedded pages) — the notebook explains the fallback (open the link directly).

## Data & Sources Used

| Source | Used for |
|---|---|
| GeoLibre live web app | Primary "quick intro" platform |
| `https://data.source.coop/giswqs/opengeos/countries.parquet` | Public, cloud-native world-countries layer (GeoLibre's own tutorial dataset) for the Visualize step |
| Esri World Imagery basemap (via `leafmap`) | Python preview map |
| NM RGIS Clearinghouse — https://rgis.unm.edu/ | Referenced as the course's ongoing regional data source (used starting Week 4) |

No student data collection or downloads happen this week — that begins in Week 4 (Lab 3: Acquire Data).

## Assessment / Submission

This is a **practice activity, not graded**. Students submit (to the LMS discussion space):
1. A screenshot from each platform tried, showing a labeled marker at WNMU / downtown Silver City
2. A short (3–5 sentence) written reflection comparing the platforms and revisiting EQ1

## Notes for the Instructor

- Swap the placeholder region-photo comment near the top of the notebook (`<!-- Optional: add a local photo... -->`) for an actual image once one is selected; keep it captioned and alt-texted per the course's UDL commitments.
- If ArcGIS Pro access isn't provisioned before Week 1 begins, the notebook's structure still works with just GeoLibre + QGIS — flag that in the live announcement rather than editing the lab itself.
- This lesson format (markdown-driven Geo-Inquiry steps, collapsible platform panels, light optional Python cells) is intended as the template for the remaining 11 labs — Weeks 2–12 can reuse this same `.ipynb` + `README.md` pairing.

---
*Lab format adapted from the Geo-Inquiry–structured lesson design used in [EarthInquiryLab](https://github.com/asivitskis/EarthInquiryLab).*
