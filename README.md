# Lockheed SR-71A Blackbird — 3D Modeling & Exploded-View Master Reference Pack
**Built for Claude, Astra / Astro, Opus 5.5 & Blender MCP**

> **Quick Machine Ingestion Guide (For Claude / LLM Agents):**
> * **Single-Page Web & Visual Gallery:** `https://jallison1193-crypto.github.io/sr71-blackbird-3d-reference-pack/`
> * **Structured JSON Manifest (All Direct URLs, Dimensions, Stations, Explode Vectors & Callouts):** [`sr71-reference-manifest.json`](./sr71-reference-manifest.json)
> * **Phase 1 Focus (3D Airframe, Cockpits & Exploded Subsystems):** Start with Sections `01` → `05`.
> * **Phase 2 Focus (Interactive Examination Popups & Engineering Snippets):** Use Section `06`.

---

## Pack Index & Organized Sections

| Section | File | Contents Summary |
| :--- | :--- | :--- |
| **01. Geometry, 3-Views & Fuselage Stations** | [`01-geometry-blueprints-stations.md`](./01-geometry-blueprints-stations.md) | Verified USAF/NASA principal dimensions in Imperial & Metric (`1.0 unit = 1m`), infinite-resolution `Lockheed_SR-71A_3view.svg`, `5` direct NASA Dryden NTRS technical report PDFs, Lockheed `FS` / `BL` / `WL` coordinate station table (`FS 200` → `FS 1489`), nacelle toe-in/droop & chine nuances. |
| **02. 3D Scans, Photogrammetry & Open Meshes** | [`02-3d-scans-and-meshes.md`](./02-3d-scans-and-meshes.md) | **CC0 Public Domain** downloadable 3D mesh of IWM Duxford SR-71A `61-7962` (`186k` tris), **GRADD 199-photo RealityCapture J58 scan** (`2.5M` tris), Polycam LiDAR capture, **GPL-2.0 `FGMEMBERS/Lockheed-SR71` repo** (`104` files with articulated surfaces + `13` 3D cockpit gauges), downloadable `262k`-face J58 mesh, and `5.3M`-tri skeletal rib/spar reference. |
| **03. Exterior Multi-Angle Photos** | [`03-exterior-multi-angle-photos.md`](./03-exterior-multi-angle-photos.md) | `25+` direct high-resolution (`2,000 px` – `6,000 px`) unauthenticated image URLs organized by **Front/Head-On**, **Top/Dorsal Planform**, **Side/3-Quarter**, **Underside/Silver Landing Gear**, **Nose Chine**, and **Rear/Afterburner Ejector Nozzles**. |
| **04. Pilot & RSO Cockpits + Flight Manual** | [`04-cockpit-pilot-and-rso.md`](./04-cockpit-pilot-and-rso.md) | Interactive **360° Front Pilot & Rear RSO Cockpit Virtual Tours** (USAF Museum), **3 direct declassified `T.O. 1SR-71A-1` Flight Manual PDFs** (`109 MB` total, OCR text-searchable), and `20+` studio fill-flash & museum hi-res photos of Pilot/RSO instrument panels, throttles, Triple Display Indicator, and Weber zero-zero ejection seats. |
| **05. Inner Workings, J58 Cutaways & Exploded Rig** | [`05-inner-workings-cutaways-exploded-rig.md`](./05-inner-workings-cutaways-exploded-rig.md) | Vector SVG & Flight Manual airflow cutaways (`Mach 0` → `Mach 3.2`), Titanium vs. Composite structural map, `12+` ultra-hi-res (`up to 32 MP`) bare **Pratt & Whitney J58** photos showing the `6` external bleed-bypass pipes, **Hycon TEOC** chine cameras, internal milled titanium ribs, and a complete **10-Collection Blender MCP Exploded-View Rig Spec** (`Explode_Factor` `0.0` → `1.0`). |
| **06. Interactive Callouts & Subsystem Lore** | [`06-callout-snippets-and-lore.md`](./06-callout-snippets-and-lore.md) | `12` ready-to-bind inspection hotspot cards mapped 1:1 to the Blender collection names—covering Beta-titanium thermal expansion, `54%` inlet spike thrust recovery, J58 bleed-bypass + `TEB` green chemical ignition, `JP-7` fuel heat-sink routing, `"R2-D2"` daylight star-tracker, and nitrogen-pressurized aluminum tires. |

---

## Executive Visual Preview (Direct Embedded References)

### Orthographic 3-View & J58 Supersonic Bleed-Bypass Cutaway
| Baseline SR-71A 3-View (`SVG`) | Pratt & Whitney J58 Airflow Cutaway (`Mach 0` → `3.2` `SVG`) |
| :---: | :---: |
| ![SR-71A 3-View](https://upload.wikimedia.org/wikipedia/commons/f/ff/Lockheed_SR-71A_3view.svg) | ![J58 Airflow Cutaway](https://upload.wikimedia.org/wikipedia/commons/8/89/SR71_J58_Engine_Airflow_Patterns.svg) |

### Key Exterior, Cockpit & Bare J58 Engine Ground-Truth Photos
| Head-On Ramp Cross-Section (`NASA SR-71B`) | Dorsal Planform & Wing Corrugations (`NASA 831`) |
| :---: | :---: |
| ![Head-On View](https://upload.wikimedia.org/wikipedia/commons/1/1c/This_photo_shows_a_head-on_view_of_NASA%27s_SR-71B_on_the_ramp_at_the_Air_Force%27s_Plant_42_in_Palmdale%2C_California%2C_shortly_before_delivery_to_DFRC_%28EC91-0365-7%29.jpg) | ![Dorsal View](https://upload.wikimedia.org/wikipedia/commons/9/97/Lockheed_SR-71_Blackbird.jpg) |
| **Forward Pilot Cockpit (`USAF Museum`)** | **Bare Pratt & Whitney J58 & 6 Bypass Tubes (`Intrepid`)** |
| ![Pilot Cockpit](https://media.defense.gov/2007/Jan/16/2000521412/2000/2000/0/070116-F-1234S-013.JPG) | ![Bare J58 Engine](https://upload.wikimedia.org/wikipedia/commons/3/38/At_the_Intrepid_Museum_2023_122.jpg) |

---

## Recommended Workflow for Claude → Astro / Opus 5.5 + Blender MCP

1. **Ingest [`sr71-reference-manifest.json`](./sr71-reference-manifest.json) + [`01-geometry-blueprints-stations.md`](./01-geometry-blueprints-stations.md):** Lock scene scale (`32.741 m` length, `16.942 m` span, `5.639 m` height, `±4.115 m` nacelle X-offset, `15°` inward rudder cant) and load `Lockheed_SR-71A_3view.svg` onto orthographic reference empties.
2. **Import Proportion & Subsystem Ground-Truth ([`02-3d-scans-and-meshes.md`](./02-3d-scans-and-meshes.md)):** Pull the CC0 Duxford `61-7962` `.glb` mesh and `FGMEMBERS/Lockheed-SR71` instrument/control sub-meshes as spatial templates; cross-check chine curvature, `~1.5°` nacelle toe-in, and `~2.5°` nacelle nose-down droop against [`03-exterior-multi-angle-photos.md`](./03-exterior-multi-angle-photos.md).
3. **Model Internal Bay & Cockpit Detail ([`04`](./04-cockpit-pilot-and-rso.md) & [`05`](./05-inner-workings-cutaways-exploded-rig.md)):** Build the 10-collection exploded-view hierarchy (`Nose_Recon_Module`, `Cockpit_Crew_Module`, `Avionics_And_Chine_Bays`, `Fuselage_JP7_Fuel_System`, `Fuselage_Titanium_Skeleton`, `Inner_And_Outer_Wings`, `Left/Right_Propulsion_Pod` with translating spike + J58 6-pipe bypass core + blow-in ejector nozzle, `Flight_Control_Surfaces`, and `Landing_Gear_Assemblies`) rigged to a master `Explode_Factor` (`0.0` → `1.0`) driver.
4. **Attach Interactive Examination Snippets ([`06-callout-snippets-and-lore.md`](./06-callout-snippets-and-lore.md)):** Bind the 12 subsystem hotspot cards to each Blender collection empty for Phase-2 interactive exploration.
