# Lockheed SR-71A Blackbird — Single-File Master Reference Packet (For Claude / Astro / Blender MCP)
> **Note:** This single file consolidates all geometry, fuselage station coordinates (`FS/BL/WL`), 3D scans/meshes, multi-angle exterior & cockpit photos, Pratt & Whitney J58 inner-workings cutaways, Blender exploded-view rig vectors, and Phase-2 interactive callout snippets so Claude can read the entire packet from **one URL**.
> * **Full Visual GitHub Repository:** https://github.com/jallison1193-crypto/sr71-blackbird-3d-reference-pack
> * **Interactive GitHub Pages Gallery:** https://jallison1193-crypto.github.io/sr71-blackbird-3d-reference-pack/
> * **Raw JSON Manifest:** https://raw.githubusercontent.com/jallison1193-crypto/sr71-blackbird-3d-reference-pack/main/sr71-reference-manifest.json

---

## PART 1: Master Principal Dimensions & Coordinate Rig (`1.0 Blender Unit = 1.0 Meter`)

| Parameter | Imperial (USAF / Lockheed) | Metric (Blender Scene Units) | Critical Modeling Notes |
| :--- | :--- | :--- | :--- |
| **Overall Length (Airframe, excl. nose pitot)** | `107 ft 5 in` (`1,289.0 in`) | **`32.741 m`** | `FS 200.0` nose radome tip to `FS 1489.0` aft tailcone |
| **Physical Wingspan** | `55 ft 7 in` (`667.0 in`) | **`16.942 m`** | NASA aero reference span `b = 17.282 m`; MAC `11.491 m` |
| **Overall Height (ground to rudder tip)** | `18 ft 6 in` (`222.0 in`) | **`5.639 m`** | Twin all-moving rudders canted **`15.0°` inward** |
| **Wheelbase / Wheel Track** | `37 ft 10 in` / `16 ft 8 in` | **`11.532 m` / `5.080 m`** | Twin nose wheels; 3-wheel aluminum-impregnated silver main bogies |
| **Outer Wing Sweep & Elevon Rigging** | `60.0°` LE sweep | **`60.0°`** | Conical camber droop on outer LE; outboard elevons **`+3.0°` TE-up** |
| **Engine Nacelle Spanwise Offset** | `BL ±162 in` (`~13.5 ft`) | **`±4.115 m` from `X = 0`** | **CRITICAL:** Nacelles toe inward **`~1.5°`** & droop **`~2.5°` nose-down**! |
| **Pratt & Whitney J58 Core Dimensions** | `180 in` L × `50 in` Dia | **`4.572 m` L × `1.270 m` Dia** | Translating inlet spike travels **`26.0 in` (`0.660 m`)** axially |

### Fuselage Station (`FS`) Axial Breakdown for Internal Slicing
* **`FS 200.0` (`0.00 m` from nose):** Nose radome tip; **`FS 295.0` (`2.41 m`):** Detachable modular nose cone bulkhead (`OBC` panoramic camera or `ASARS-1` radar).
* **`FS 295 – 375` (`2.41 – 4.45 m`):** Forward lateral chine bays (`Hycon TEOC` optical cameras & `ELINT`).
* **`FS 375 – 465` (`4.45 – 6.73 m`):** **Forward Pilot Cockpit** (V-shaped quartz windscreen, `TDI` gauge, Weber zero-zero ejection seat).
* **`FS 465 – 545` (`6.73 – 8.76 m`):** **Aft RSO Cockpit** (twin side windows, optical belly viewfinder, radar/nav consoles, RSO Weber seat).
* **`FS 545 – 605` (`8.76 – 10.29 m`):** **Nortronics `NAS-14V2` Astro-Inertial Star-Tracker ("R2-D2")** beneath dorsal quartz window + Nose Gear Well below.
* **`FS 605 – 715` (`10.29 – 13.08 m`):** **Fuel Tank 1**, belly sensor bays, `FS 683` gyro bay, **`FS 715.0` primary wing-fuselage carry-through bulkhead**, and dorsal refueling receptacle.
* **`FS 715 – 942` (`13.08 – 18.85 m`):** **Fuel Tanks 2, 3 & 4** + forward inlet spikes & nacelle cowls outboard at `X = ±4.115 m`.
* **`FS 942 – 1080` (`18.85 – 22.35 m`):** **Main Landing Gear Wells** (retract inward into fuselage/inner wing), **Fuel Tank 5**, and **J58 9-stage compressor/turbine cores**.
* **`FS 1080 – 1260` (`22.35 – 26.92 m`):** **Fuel Tank 6A (Aft CG Trim Tank)**, **J58 Afterburners**, and **Twin `15°` Inward-Canted All-Moving Rudders** (`FS 1135` mid-tail station).
* **`FS 1260 – 1489` (`26.92 – 32.74 m`):** **Free-Floating Blow-In Door Ejector Nozzles**, **Inboard/Outboard Elevons**, and **Dorsal Drag-Chute Bay**.

---

## PART 2: Orthographic 3-Views, Flight Manuals & NASA NTRS Engineering PDFs

* **Infinite-Resolution Orthographic 3-View Vector (`SVG`):** https://upload.wikimedia.org/wikipedia/commons/f/ff/Lockheed_SR-71A_3view.svg
* **NASA/Lockheed 3-View Line Drawing (`PNG`):** https://upload.wikimedia.org/wikipedia/commons/b/b3/Lockheed_SR-71B_trainer_model_3view.png
* **Declassified USAF `T.O. 1SR-71A-1` Flight Manual (OCR Searchable PDFs):**
  * **Part 1 (Airframe, Pilot/RSO Panels, Fuel Heat-Sink Fig. 1-4, Spike Fig. 1-7, J58 Cutaway Fig. 1-21):** https://archive.org/download/0003756-lockheed-sr-71-03/SR-71%20Flight%20Manual/0003756-lockheed_sr71__01_text.pdf
  * **Part 2 (Operating Procedures):** https://archive.org/download/0003756-lockheed-sr-71-03/SR-71%20Flight%20Manual/0003756-lockheed_sr71__02_text.pdf
  * **Part 3 (Section 4 `ANS` Star-Tracker, Cooling & Performance):** https://archive.org/download/0003756-lockheed-sr-71-03/SR-71%20Flight%20Manual/0003756-lockheed_sr71__03_text.pdf
* **NASA Dryden Technical Reports (Direct PDFs):**
  * `NASA/TP-2000-209023` (*SR-71 Test Bed Aircraft — 3-Views & Stations*): https://ntrs.nasa.gov/api/citations/20000064011/downloads/20000064011.pdf
  * `NASA/TP-2002-210718` (*Stability & Control — Geometry & Surfaces*): https://ntrs.nasa.gov/api/citations/20020057965/downloads/20020057965.pdf
  * `AIAA 2009-1522` (*Design & Development — Titanium & Composite Structure*): https://ntrs.nasa.gov/api/citations/20090007797/downloads/20090007797.pdf
  * `NASA-TM-X-3099` (*YF-12C / SR-71A J58 Nacelle & Spike Stations*): https://ntrs.nasa.gov/api/citations/19740024172/downloads/19740024172.pdf

---

## PART 3: 3D Scans, Photogrammetry & Open-Source Sub-Assemblies

1. **CC0 Public Domain Downloadable Museum Mesh — SR-71A `61-7962` (IWM Duxford, `186,323` tris):** https://sketchfab.com/3d-models/sr-71a-blackbird-61-7962-duxford-00c24dd3549a4f429dd1a0a2469e9ba4
2. **GRADD 199-Photo RealityCapture Photogrammetry Scan — Bare Pratt & Whitney J58 (`2.5M` tris, Museum of Flight Seattle):** https://sketchfab.com/3d-models/gradd-sr-71-blackbird-a12-j58-engine-3d-model-9fe852b2c84b442bb112aec9c8c8b29e
3. **Polycam LiDAR / Photogrammetry Capture (San Diego Blackbird):** https://poly.cam/capture/02BE69A5-AED5-43CF-8536-8B8435C541CF
4. **Open-Source `FGMEMBERS/Lockheed-SR71` (`GPL-2.0`, `104` files — articulated `.ac` meshes + `13` 3D cockpit gauges):** https://github.com/FGMEMBERS/Lockheed-SR71 *(Sketchfab `.glb` mirror: https://sketchfab.com/3d-models/lockheed-sr-71-blackbird-1850c7bb7ac54902bd9868381ff8b652)*
5. **Downloadable High-Poly Pratt & Whitney J58 Engine Mesh (`262,638` faces, `CC BY-NC-SA`):** https://sketchfab.com/3d-models/j58-jet-engine-bca3015516304cfabe249cfad5363939
6. **Skeletal Blackbird (`5.3M` tris — Internal Rib/Bulkhead Layout Reference):** https://sketchfab.com/3d-models/skeletal-blackbirdsr-71-skeleton-ac3ed6faf9094ead90dabe22aceba2b7
7. **Individual 3D Cockpit Controls & Gauges (`Cesar.Ferrolho`):**
   * Flightstick: https://sketchfab.com/3d-models/sr-71-flightstick-448d8f5727af4f05b1017f6e6fb33587
   * Triple Display Indicator (`TDI`): https://sketchfab.com/3d-models/sr-71-triple-display-indicator-second-version-da9d101f8c3844fe9da1f7cb5475e156
   * Attitude Indicator (`ADI`): https://sketchfab.com/3d-models/sr-71-attitude-indicator-3f2883f756a24efc80eb984f6e7c0055

---

## PART 4: High-Resolution Exterior, Cockpit & Inner-Workings Direct Image URLs

### Exterior All-Angles
* **Pure Head-On Ramp Cross-Section (`3000×2400`):** https://upload.wikimedia.org/wikipedia/commons/1/1c/This_photo_shows_a_head-on_view_of_NASA%27s_SR-71B_on_the_ramp_at_the_Air_Force%27s_Plant_42_in_Palmdale%2C_California%2C_shortly_before_delivery_to_DFRC_%28EC91-0365-7%29.jpg
* **Front-Quarter Udvar-Hazy Chine View (`3872×2592`):** https://upload.wikimedia.org/wikipedia/commons/2/21/NASM_-_SR-71_Blackbird_2.jpg
* **Overhead Dorsal Planform (`2100×2400`):** https://upload.wikimedia.org/wikipedia/commons/5/55/Linear_Aerospike_SR-71_Experiment_%28LASRE%29_first_flight_view_from_above_%28EC97-44295-84%29.jpg
* **20 MP Dorsal Wing Corrugations & Sawtooth Chines (`5100×3996`):** https://upload.wikimedia.org/wikipedia/commons/9/97/Lockheed_SR-71_Blackbird.jpg
* **Side Landing Profile, Gear Stance & Drag Chute (`5100×4000`):** https://upload.wikimedia.org/wikipedia/commons/4/4a/SR-71_Landing_with_Drag_Chute_-_GPN-2000-001944.jpg
* **Baseline SR-71A Clean Dorsal Spine Side View (`61-7971`):** https://upload.wikimedia.org/wikipedia/commons/5/54/Lockheed_SR-71A_61-7971%2C_Edwards_AFB%2C_CA_Oct96_%2852302789562%29.jpg
* **Translating Inlet Spike Macro (`5184×3456`):** https://upload.wikimedia.org/wikipedia/commons/b/bc/Lockheed_SR-71_left_engine_spike_%286586704831%29_%285%29.jpg
* **Main Gear Strut & 3-Wheel Bogie (`3000×4000`):** https://upload.wikimedia.org/wikipedia/commons/b/b5/Lockheed_SR-71_Blackbird_-_Landing_Gear_%284889948402%29.jpg
* **Aluminum-Impregnated Silver Main Tires (`5023×3413`):** https://upload.wikimedia.org/wikipedia/commons/1/1f/Tires_-_Lockheed_SR-71A_Blackbird%2C_1966_-_Evergreen_Aviation_%26_Space_Museum_-_McMinnville%2C_Oregon_-_DSC01031.jpg
* **Ventral Belly, Nose Gear & Sensor Doors (`6000×4000`):** https://upload.wikimedia.org/wikipedia/commons/e/ea/SR-71_Landing_Gear_and_Entry_Door_%2849071408071%29.jpg
* **Rear Blow-In Door Ejector Nozzle (`3384×2511`):** https://upload.wikimedia.org/wikipedia/commons/2/2a/Lockheed_SR-71_jet_exhaust_detail%2C_National_Museum_of_the_US_Air_Force%2C_Dayton%2C_Ohio%2C_USA._%2831485223097%29.jpg
* **Internal Afterburner Flameholder & Nozzle (`2700×1800`):** https://upload.wikimedia.org/wikipedia/commons/b/bc/Blackbird_SR-71_engine_nozzle.jpg

### Pilot & RSO Cockpits + 360° Tours
* **360° Pilot Front Cockpit Tour:** http://www.nmusafvirtualtour.com/media/068/SR-71A%20Front%20Cockpit.html
* **360° RSO Rear Cockpit Tour:** http://www.nmusafvirtualtour.com/media/068/SR-71A%20Rear%20Cockpit.html
* **Pilot Main Panel (`Hi-Res`):** https://media.defense.gov/2007/Jan/16/2000521412/-1/-1/0/070116-F-1234S-013.JPG
* **Pilot Left Console, Throttles & Spike Controls (`Hi-Res`):** https://media.defense.gov/2010/May/10/2000521423/-1/-1/0/070116-F-1234S-010.JPG
* **Pilot Center Pedestal & Stick (`Hi-Res`):** https://media.defense.gov/2007/Jan/16/2000521421/-1/-1/0/070116-F-1234S-011.JPG
* **Pilot Right Console, Fuel/CG & Master Caution (`Hi-Res`):** https://media.defense.gov/2007/Jan/16/2000521414/-1/-1/0/070116-F-1234S-012.JPG
* **RSO Rear Cockpit Panel & Viewfinder (`Hi-Res`):** https://media.defense.gov/2020/Feb/25/2002254473/-1/-1/0/200225-F-IO108-001.JPG
* **Weber Ejection Seat & Gold Canopy Cylinder (`3502×2398`):** https://upload.wikimedia.org/wikipedia/commons/b/bb/SR-71_Systems_operators_cockpit%2C_controls%2C_instruments%2C_ejection_seat_%284527964406%29.jpg

### Cutaways, J58 Bleed-Bypass Engine & Internal Sensors
* **J58 Internal Nacelle Cutaway (`Mach 0` → `3.2` `SVG`):** https://upload.wikimedia.org/wikipedia/commons/8/89/SR71_J58_Engine_Airflow_Patterns.svg
* **J58 Mach 3 Shockwave Trap Cross-Section (`PNG`):** https://upload.wikimedia.org/wikipedia/commons/1/1b/J58_airflow_at_Mach_3.png
* **85% Titanium vs. 15% Composite Structural Map (`GIF`):** https://upload.wikimedia.org/wikipedia/commons/8/85/Sr-71-composit.gif
* **32 MP Bare J58 Engine & 6 External Bleed-Bypass Pipes (`6960×4640`):** https://upload.wikimedia.org/wikipedia/commons/3/38/At_the_Intrepid_Museum_2023_122.jpg
* **USAF Museum Bare J58 Rigging Photos (`Hi-Res`):** https://media.defense.gov/2020/May/14/2002300185/-1/-1/0/200513-F-IO108-045.JPG & https://media.defense.gov/2020/May/14/2002300187/-1/-1/0/200513-F-IO108-047.JPG
* **Hycon `TEOC` No. 36 Chine Optical Camera (`5472×3648`):** https://upload.wikimedia.org/wikipedia/commons/c/c8/Technical_Objective_Camera_%28TEOC%29%2C_No._36%2C_Hycon_Corporation_-_Lockheed_SR-71A_Blackbird%2C_1966_-_Evergreen_Aviation_%26_Space_Museum_-_McMinnville%2C_Oregon_-_DSC01063.jpg
* **Internal Milled Titanium Ribs & Fasteners (`7535×4088`):** https://upload.wikimedia.org/wikipedia/commons/1/1c/SR-71_61-7953_debris_1.jpg

---

## PART 5: Blender MCP Exploded-View Hierarchy & Phase-2 Examination Callouts

Bind custom property `Explode_Factor` (`0.0` → `1.0`) on `SR71_Master_Root` to drive local separation of **10 collections**, each linked to a Phase-2 callout card:
1. **`01_Nose_Recon_Module`** (`-3.5m` axial): Detachable `FS 295` nose pod housing either the **Itek Optical Bar Camera** (`10,500 ft` panoramic film) or **Loral `ASARS-1` Synthetic Aperture Radar**.
2. **`02_Cockpit_Crew_Module`** (Canopies `+2.2m Z / +35°`, Weber seats `+3.8m Z`): Quartz V-windscreen (`640 °F` exterior), Pilot `TDI` (`KEAS/Mach/Alt`), and RSO sensor/EW station surveying `100,000 sq mi/hr` from `85,000 ft`.
3. **`03_Avionics_And_Chine_Bays`** (`ANS +1.6m Z`, `TEOC ±2.0m X`): **Nortronics `NAS-14V2` ("R2-D2")** daylight blue-light star-tracker (`61` stars, `~300 ft` accuracy) + sharp radar-absorbing sawtooth composite chines generating supersonic vortex lift.
4. **`04_Fuselage_JP7_Fuel_System`** (`Tanks 1–6A` translucent amber volumes): `~80,000 lb` of `140 °F`-flashpoint **JP-7** acting as the aircraft's thermal **heat sink** (cooling cockpits, avionics, hydraulics & oil before burning at `300 °F`) and longitudinal Mach 3 CG trim.
5. **`05_Fuselage_Titanium_Skeleton`** (Dorsal skin `+3.2m Z`, Belly `-2.4m Z`): `85%` `Ti-13V-11Cr-3Al` Beta-titanium milled ring bulkheads with primary wing carry-through at `FS 715.0`.
6. **`06_Inner_And_Outer_Wings`** (Corrugated skins `±2.0m Z`, Sawtooth edges `±2.8m X`): Chordwise stamped thermal-expansion corrugations accommodating `450–600 °F` airframe growth, with zero fuel stored in the outer wings.
7. **`07_Left_Propulsion_Pod` & `08_Right_Propulsion_Pod`** (Spike `-4.5m` forward, Cowls `±2.6m Z`, Ejector `+4.2m` aft): Computer-scheduled `26-inch` translating spike (`~54%` of Mach 3.2 thrust via shockwave pressure recovery!) + **Pratt & Whitney J58** (`32,500 lbf` thrust, **6 external 4th-stage bleed-bypass pipes** feeding the afterburner, **Triethylborane `TEB`** green pyrophoric ignition) + free-floating blow-in door ejector (`~28.4%` thrust).
8. **`09_Flight_Control_Surfaces`** (Rudders `+2.8m`, Elevons `+2.0m` aft): Twin `15°` inward-canted **all-moving rudders** (massive yaw authority for Mach 3 inlet unstarts) + inboard/outboard elevons (`+3°` outboard TE-up rigging).
9. **`10_Landing_Gear_Assemblies`** (`-2.2m Z`): `22-ply` **aluminum-powder-impregnated metallic silver B.F. Goodrich tires** pressurized to `415 psi` with dry nitrogen to survive `550 °F` wheel wells and `175+ kt` landings.
