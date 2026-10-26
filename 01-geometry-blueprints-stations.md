# Section 01: Geometry, 3-Views, Fuselage Stations & Structural Reference
## Lockheed SR-71A Blackbird — Authoritative Blender Scale & Coordinate Spec

> **Purpose for Astra / Opus 5.5 + Blender MCP:** Use these verified NASA Dryden / USAF `T.O. 1SR-71A-1` dimensions and Fuselage Station (`FS`) coordinates as the master scene rig before blocking out or importing any mesh. Set Blender scene units to **Metric (`1.0 unit = 1.0 meter`)**, aircraft nose pointing along **`-Y`** (or `+Y` per rig convention; below maps `FS` inches directly to meters from the nose datum).

---

## 1. Master Principal Dimensions (SR-71A)

| Parameter | Imperial (USAF / Lockheed) | Metric (Blender Scene Units) | Source |
| :--- | :--- | :--- | :--- |
| **Overall Length (Airframe, excl. nose pitot boom)** | `107 ft 5 in` (`1,289.0 in`) | **`32.741 m`** | USAF Fact Sheet / `T.O. 1SR-71A-1` |
| **Overall Length (incl. nose pitot boom)** | `107 ft 5 in` + pitot (~`3 ft 1 in` probe) | ~`33.68 m` (verify against 3-view SVG) | Lockheed general arrangement |
| **Physical Wingspan** | `55 ft 7 in` (`667.0 in`) | **`16.942 m`** | USAF Fact Sheet / `T.O. 1SR-71A-1` |
| **NASA Aerodynamic Reference Span ($b$)** | `56.70 ft` | **`17.282 m`** | `NASA/TM-1998-206567` / `NASA/TP-2002-210718` |
| **Mean Aerodynamic Chord ($\bar{c}$)** | `37.70 ft` | **`11.491 m`** | `NASA/TM-1998-206567` |
| **Reference Wing Area ($S$)** | `1,605 sq ft` (planform `1,800 sq ft`) | **`149.11 m²`** (`167.23 m²` total delta) | NASA Dryden / Lockheed |
| **Overall Height (ground to rudder tip)** | `18 ft 6 in` (`222.0 in`) | **`5.639 m`** | USAF Fact Sheet / `T.O. 1SR-71A-1` |
| **Wheelbase (Nose Gear to Main Gear)** | `37 ft 10 in` (`454.0 in`) | **`11.532 m`** | Lockheed SR-71A Spec |
| **Wheel Track (Left Main to Right Main)** | `16 ft 8 in` (`200.0 in`) | **`5.080 m`** | Lockheed SR-71A Spec |
| **Outer Wing Leading-Edge Sweep** | `60.0°` (sharp nose-chine transition forward) | **`60.0°`** (with conical camber on outer LE) | `NASA/TP-2000-209023` |
| **Twin All-Moving Rudder Cant Angle** | `15.0°` **inward** toward centerline | **`15.0°` inward** (pivots atop nacelles) | `T.O. 1SR-71A-1` |
| **Engine Nacelle Centerline Spanwise Offset** | `BL ±162 in` (~`13.5 ft` from centerline) | **`±4.115 m` from `X = 0`** | NASA Dryden YF-12C / SR-71 layout |
| **Nacelle Diameter (max outer cowl)** | ~`5 ft 6 in` (`66 in` nominal around J58) | ~**`1.676 m`** | J58 `50 in` engine + bypass ducts |
| **Outboard Elevon Rigging Incidence** | `3.0°` trailing-edge-up relative to inboard | **`+3.0°` TE-up** | `NASA/TM-1998-206567` |

---

## 2. Verified 3-View Vector & NASA Engineering Drawings

### Primary Orthographic 3-View (SVG Vector — Direct Download)
* **Wikimedia Commons Vector 3-View (`Lockheed_SR-71A_3view.svg`):**
  * **Direct SVG URL:** https://upload.wikimedia.org/wikipedia/commons/f/ff/Lockheed_SR-71A_3view.svg
  * **Resolution / Type:** Infinite-resolution `image/svg+xml` (`1854 × 1419` viewbox), Public Domain.
  * **Blender MCP Usage:** Convert or rasterize at `8192 px` width and place on Top (`XY`), Side (`YZ`), and Front (`XZ`) reference empty planes scaled so fuselage length equals `32.741 m`.

### Primary NASA Technical Reports with Engineering 3-Views, Stations & Cross-Sections (Direct PDFs)
1. **NASA/TP-2000-209023 — *The SR-71 Test Bed Aircraft: A Facility for High-Speed Flight Research***
   * **Direct PDF:** https://ntrs.nasa.gov/api/citations/20000064011/downloads/20000064011.pdf
   * **Citation Page:** https://ntrs.nasa.gov/citations/20000064011
   * **Key Modeling Content:** Baseline SR-71A 3-view schematic drawings, nose/chine payload bay geometry, dorsal payload hardpoints, fuselage station thermal & structural load distributions (`FS 683`, `FS 942`, `FS 1038`, `FS 1135`).
2. **NASA/TP-2002-210718 — *Stability and Control Estimation Flight Test Results for the SR-71 Aircraft With Externally Mounted Experiments***
   * **Direct PDF:** https://ntrs.nasa.gov/api/citations/20020057965/downloads/20020057965.pdf
   * **Citation Page:** https://ntrs.nasa.gov/citations/20020057965
   * **Key Modeling Content:** Figures 1–3 baseline SR-71A geometry, control surface breakdown (inboard elevons, outboard elevons, twin all-moving rudders), and exact `FS` / `BL` / `WL` coordinate system definitions.
3. **NASA/TM-1998-206567 — *Flight Stability and Control and Performance Results from the Linear Aerospike SR-71 Experiment (LASRE)***
   * **Direct PDF:** https://ntrs.nasa.gov/api/citations/19980231067/downloads/19980231067.pdf
   * **Key Modeling Content:** Geometric nomenclature ($b = 56.7\text{ ft}$, $\bar{c} = 37.7\text{ ft}$), structural attachment points, elevon/rudder rigging angles.
4. **AIAA 2009-1522 (Peter W. Merlin, NASA Dryden) — *Design and Development of the Blackbird: Challenges and Lessons Learned***
   * **Direct PDF:** https://ntrs.nasa.gov/api/citations/20090007797/downloads/20090007797.pdf
   * **Key Modeling Content:** Structural material map (`85%` Titanium `Ti-13V-11Cr-3Al` Beta-alloy & `Ti-6Al-4V`, `15%` high-temperature phenyl-silane / asbestos-laminate radar-absorbing composite chines and trailing edges), corrugations/chordwise thermal expansion bead patterns on upper/lower wing skins.
5. **NASA-TM-X-3099 — *Description of YF-12C Airplane, Propulsion System, and Instrumentation for Propulsion Research Flight Tests***
   * **Direct PDF:** https://ntrs.nasa.gov/api/citations/19740024172/downloads/19740024172.pdf
   * **Key Modeling Content:** Note: "YF-12C" (`61-7951`) was actually an **SR-71A airframe** loaned to NASA under a cover designation! This report contains detailed J58 nacelle station diagrams, translating spike travel (`26 inches` axial translation), forward/aft bypass doors, suck-in doors, and ejector nozzle geometry.

---

## 3. Lockheed Coordinate System (`FS`, `BL`, `WL`) for Sub-Assembly Placement

Lockheed's engineering datum defines coordinates in **inches**:
* **Fuselage Station (`FS`):** Longitudinal distance aft from a virtual datum ahead of the nose (`FS 200.0` ≈ nose radome tip on standard SR-71A station charts; aft tailcone / drag-chute fairing terminates near `FS 1489.0`, spanning `1,289 in = 107 ft 5 in`).
* **Butt Line (`BL`):** Lateral distance left/right from fuselage centerline (`BL 0.0`).
* **Water Line (`WL`):** Vertical height above horizontal reference plane below the belly (`WL 100.0` ≈ fuselage chine/reference horizontal plane).

### Documented Axial Stations & Structural Bulkheads
| Station (`FS` in) | Metric Offset from Nose Tip (`FS - 200` × `0.0254 m`) | Component / Internal Feature (for Exploded View Slicing) |
| :--- | :--- | :--- |
| **`FS 200.0`** | `0.00 m` | Nose cone radome tip (detachable Nose Bay — Optical Bar Camera / Radar) |
| **`FS 295 – 375`** | `2.41 – 4.45 m` | Detachable Nose Cone Bulkhead & Forward Chine Equipment Bays (`E` / `F` bays) |
| **`FS 375 – 465`** | `4.45 – 6.73 m` | **Forward Cockpit (Pilot Station)**: clamshell V-windscreen, instrument shroud, Weber zero-zero ejection seat |
| **`FS 465 – 545`** | `6.73 – 8.76 m` | **Aft Cockpit (RSO Station)**: twin small side windows, sensor/navigation consoles, RSO ejection seat |
| **`FS 545 – 605`** | `8.76 – 10.29 m` | **Nortronics NAS-14V2 Astro-Inertial Navigation System (ANS)** ("R2-D2" star-tracker behind RSO, viewing sky through dorsal quartz window) + Forward Nose Gear Well below |
| **`FS 605 – 683`** | `10.29 – 12.27 m` | **Fuel Tank 1** (forward fuselage tank) + lower fuselage sensor/camera bays (`A/B/C` bays) & `FS 683.0` (`BL 32.5, WL 86.2`) gyro/accelerometer bay |
| **`FS 715.0`** | `13.08 m` | **Primary Wing-to-Fuselage Structural Carry-Through Joint** & **Fuel Tank 2** + Dorsal In-Flight Refueling Receptacle |
| **`FS 780 – 942`** | `14.73 – 18.85 m` | **Fuel Tank 3 & Tank 4** (integral titanium fuselage tanks) + **Inlet Spike Tip & Forward Nacelle Cowls** outboard at `BL ±162` |
| **`FS 942 – 1080`** | `18.85 – 22.35 m` | **Main Landing Gear Bays** (retract inward into fuselage/wing root; 3-wheel titanium-impregnated silver tires per bogie), **Fuel Tank 5**, and **Pratt & Whitney J58 Core Compressor/Turbine** |
| **`FS 1080 – 1260`** | `22.35 – 26.92 m` | **Fuel Tank 6A (Aft Trim Tank)**, **J58 Afterburner Ducts**, and **Twin All-Moving Cantilevered Rudders** (`FS 1135` mid-tail thermal station) |
| **`FS 1260 – 1489`** | `26.92 – 32.74 m` | **Free-Floating Blow-In Door Ejector Nozzles**, **Inboard/Outboard Elevons**, and **Aft Tailcone / Drag Parachute Compartment** |

---

## 4. Key Airframe Surface & Silhouette Nuances (Critical for Accuracy)

1. **Blended Chine Cross-Section ("Cobra Hood"):**
   * The forward fuselage is **not** a simple cylinder: lateral sharp chines blend smoothly from the nose tip all the way into the `60°` delta wing leading edge, generating vortex lift at supersonic speeds and reducing radar cross-section.
2. **Inward Engine Nacelle Toe-In & Downward Droop:**
   * The J58 inlet nacelles are **toed inward slightly toward the fuselage centerline** (~`1.2°–1.5°` toe-in) and **drooped downward** (~`2.5°–3°` nose-down incidence) at the front so the translating inlet spikes align directly with the local Mach 3.2 under-chine shockwave/upwash flowfield! Modeling them strictly parallel to `Y` and `Z` is the #1 mistake on amateur SR-71 models.
3. **Conical Camber on Outer Wing Leading Edges:**
   * Outboard of the engine nacelles, the delta wing leading edges droop downward in a **conical camber** curve, and the wingtips curve slightly downward.
4. **Chordwise Skin Corrugations:**
   * Both upper and lower wing surfaces between the fuselage and nacelles (and outboard) feature **prominent chordwise stamped corrugations** (expansion beads) so the `Ti-13V-11Cr-3Al` skin can expand thermally at `500–600 °F` without buckling the spars. Model these via high-resolution normal/displacement maps or array-instanced bevel strips.
5. **Composite "Pie-Slice" Sawtooth Chines:**
   * Along the chine edges and wing trailing edges, triangular ("dog-tooth" / sawtooth) radar-absorbing phenyl-silane composite tiles alternate with titanium structure.
