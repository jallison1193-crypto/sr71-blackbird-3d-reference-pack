# Section 05: Inner Workings, Cutaways, J58 Bleed-Bypass Engine & Exploded-View Rig
## Complete Subsystem Reference & Blender Collection Hierarchy for Blow-Up Visualizations

> **Core Design Goal:** Enable an interactive or keyframed **"exploded cutaway"** in Blender where outer titanium/composite skins, canopies, nose radome, and nacelle cowlings separate cleanly along local axes to reveal the internal **Pratt & Whitney J58 turboramjets**, **6 external bleed-bypass ducts**, **translating inlet spike actuator**, **6 fuselage JP-7 heat-sink fuel tanks**, **Nortronics ANS star-tracker**, and **reconnaissance camera/radar bays**.

---

## 1. Cutaways, Airflow Schematics & Internal Arrangement Diagrams

| Diagram / Technical Cutaway | Format & Resolution | Direct URL |
| :--- | :--- | :--- |
| **Pratt & Whitney J58 Internal Nacelle & Airflow Cutaway (`Mach 0` → `Mach 3.2`)** *(Vectorized from `SR-71A-1` Fig. 1-21)* | Infinite SVG (`850 × 1050`) | https://upload.wikimedia.org/wikipedia/commons/8/89/SR71_J58_Engine_Airflow_Patterns.svg |
| **J58 Internal Cross-Section & Shockwave Trap at Mach 3.0** *(Flight Manual Excerpt)* | PNG (`842 × 230`) | https://upload.wikimedia.org/wikipedia/commons/1/1b/J58_airflow_at_Mach_3.png |
| **J58 / Nacelle Multi-Stage Airflow & Bypass Schematic (`SR71J58.png`)** | PNG (`1000 × 1400`) | https://upload.wikimedia.org/wikipedia/commons/0/02/SR71J58.png |
| **SR-71 Titanium vs. Composite Structural Material Map (`Sr-71-composit.gif`)** | GIF (`1000 × 801`) | https://upload.wikimedia.org/wikipedia/commons/8/85/Sr-71-composit.gif |
| **Declassified `T.O. 1SR-71A-1` Flight Manual — Part 1 (Fuel Tank Arrangement Fig. 1-4, Inlet Spike Fig. 1-7, Hydraulic & Electrical Cutaways)** | Searchable PDF (`36.1 MB`) | https://archive.org/download/0003756-lockheed-sr-71-03/SR-71%20Flight%20Manual/0003756-lockheed_sr71__01_text.pdf |
| **Declassified `T.O. 1SR-71A-1` Flight Manual — Part 3 (Section 4: ANS Astro-Inertial Star-Tracker & Environmental Cooling Schematics)** | Searchable PDF (`37.3 MB`) | https://archive.org/download/0003756-lockheed-sr-71-03/SR-71%20Flight%20Manual/0003756-lockheed_sr71__03_text.pdf |
| **Leland Haynes SR-71 Schematics & Skunk Works Executive Handbook Cutaways (Wayback Mirror)** | HTML + `13` Schematics | http://web.archive.org/web/20260208145315/http://www.wvi.com/%7Esr71webmaster/schematic.html |

---

## 2. Pratt & Whitney J58 (`JT11D-20`) Bare Engine Hardware Reference Photos (360° Plumbing & Bypass Tubes)

When the SR-71's nacelle cowlings separate in an exploded view, the **J58 engine** is the centerpiece mechanical sculpture:
* **9-stage axial compressor** with **6 massive external bleed-bypass pipes** curving from the **4th compressor stage** around the outside of the combustion section directly into the **afterburner diffuser** (at `Mach 3.2`, ~`20%` of compressor air bypasses the core turbine to burn directly in the afterburner like a ramjet, while the inlet itself provides ~`54%` of total thrust via pressure recovery).
* **Dimensions & Weight:** Length `180 in` (`4.57 m`), max diameter `50 in` (`1.27 m`), dry weight ~`6,000 lb` (`2,722 kg`), sea-level static thrust `32,500 lbf` (`144.6 kN`) with afterburner, fueled by low-volatility **JP-7** ignited chemically with **Triethylborane (TEB)**.

| Hardware View | Resolution | Direct Image URL |
| :--- | :--- | :--- |
| **Bare J58 Engine — Full Side View Showing 6 External Bleed-Bypass Pipes (`Intrepid`, `32 MP`)** | `6960 × 4640` | https://upload.wikimedia.org/wikipedia/commons/3/38/At_the_Intrepid_Museum_2023_122.jpg |
| **Bare J58 Engine Moving / Rigging Views — USAF Museum Cold War Gallery (`2` angles)** | Full Original (`-1/-1`) & `2000px` | • https://media.defense.gov/2020/May/14/2002300185/2000/2000/0/200513-F-IO108-045.JPG ([Original](https://media.defense.gov/2020/May/14/2002300185/-1/-1/0/200513-F-IO108-045.JPG)) <br>• https://media.defense.gov/2020/May/14/2002300187/2000/2000/0/200513-F-IO108-047.JPG ([Original](https://media.defense.gov/2020/May/14/2002300187/-1/-1/0/200513-F-IO108-047.JPG)) |
| **Bare J58 Engine — 3/4 Front & Compressor Bleed Valves (`4500 × 3003`)** | `4500 × 3003` | https://upload.wikimedia.org/wikipedia/commons/c/cd/18-15-112-J58.jpg |
| **Bare J58 Engine — Side Plumbing, Fuel Manifold & Afterburner Can (`4205 × 2798`)** | `4205 × 2798` | https://upload.wikimedia.org/wikipedia/commons/6/6d/SR-71_Engine_%2817473380699%29.jpg |
| **Bare J58 Engine — Aerospace Museum of California (`3` angles)** | `3456 × 2304` (×3) | • https://upload.wikimedia.org/wikipedia/commons/2/23/J-58_Engine_for_an_SR-71_Blackbird.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/6/65/J-58_Engine.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/4/40/J-58_in_the_Aerospace_Museum_of_California.jpg |
| **Bare J58 Engine — Museum of Flight Seattle & Blackbird Airpark** | `2592 × 1936` & `3264 × 2448` | • https://upload.wikimedia.org/wikipedia/commons/3/37/J58Engine_MuseumOf_Flight_Seattle.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/a/a5/SR-71A_at_Joe_Davies_Heritage_Airpark_-_J58_Jet_Engine._-_panoramio.jpg |
| **J58 Ground Test Cell Running in Full Afterburner with Shock Diamonds (`NASA EC97-44007-01`)** | `3441 × 3114` | https://upload.wikimedia.org/wikipedia/commons/e/ed/J58_Turbojet_in_Full_Afterburner_%28EC97-44007-01%29.jpg |
| **Buick Wildcat / Big-Block V8 Twin `AG330` Ground Start Cart** | `2592 × 1944` | https://upload.wikimedia.org/wikipedia/commons/7/78/AG330_start_cart.JPG |

---

## 3. Internal Reconnaissance Sensors, Optical Cameras & Structural Titanium Hardware

| Internal Subsystem | Resolution | Direct Image URL & Description |
| :--- | :--- | :--- |
| **Hycon Technical Objective Camera (`TEOC` No. 36) — Chine Bay Optical Reconnaissance Camera (`3` angles)** | `5472 × 3648` (×3) | • https://upload.wikimedia.org/wikipedia/commons/c/c8/Technical_Objective_Camera_%28TEOC%29%2C_No._36%2C_Hycon_Corporation_-_Lockheed_SR-71A_Blackbird%2C_1966_-_Evergreen_Aviation_%26_Space_Museum_-_McMinnville%2C_Oregon_-_DSC01063.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/6/6e/Technical_Objective_Camera_%28TEOC%29_detail%2C_No._36%2C_Hycon_Corporation_-_Lockheed_SR-71A_Blackbird%2C_1966_-_Evergreen_Aviation_%26_Space_Museum_-_McMinnville%2C_Oregon_-_DSC01065.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/9/9e/Technical_Objective_Camera_%28TEOC%29_detail%2C_No._36%2C_Hycon_Corporation_-_Lockheed_SR-71A_Blackbird%2C_1966_-_Evergreen_Aviation_%26_Space_Museum_-_McMinnville%2C_Oregon_-_DSC01067.jpg |
| **Internal Titanium Rib, Riveted Stringer & Honeycomb/Corrugated Structure (`61-7953` Exposed Structure Macro)** | `7535 × 4088` & `5599 × 4600` | • https://upload.wikimedia.org/wikipedia/commons/1/1c/SR-71_61-7953_debris_1.jpg <br>• https://upload.wikimedia.org/wikipedia/commons/c/c6/SR-71_-61-7953_debris_2.jpg |

---

## 4. Recommended Blender Collection Hierarchy & Exploded-View Rig Architecture

Organize the Blender MCP scene into **10 modular sub-collections** parented to `SR71_Master_Root` driven by a custom property `Explode_Factor` (`0.0` → `1.0`):

```text
SR71_Master_Root (Empty at World Origin 0,0,0; Metric 1.0 = 1m)
├── 01_Nose_Recon_Module
│   ├── Nose_Radome_Shell          [Explode: -3.5m along longitudinal axis]
│   └── OBC_SLR_Nose_Payload       [Explode: -1.8m along longitudinal axis]
├── 02_Cockpit_Crew_Module
│   ├── Forward_Canopy_Clamshell   [Explode: +2.2m Z, -0.5m Y, +35° hinge]
│   ├── Aft_RSO_Canopy_Clamshell   [Explode: +2.2m Z, +0.3m Y, +35° hinge]
│   ├── Pilot_Weber_Ejection_Seat  [Explode: +3.8m Z (vertical extraction)]
│   ├── RSO_Weber_Ejection_Seat    [Explode: +3.8m Z (vertical extraction)]
│   └── Pilot_RSO_Tub_And_Panels   [Stays at 0.0m core datum for close-up inspection]
├── 03_Avionics_And_Chine_Bays
│   ├── Nortronics_ANS_StarTracker [Explode: +1.6m Z out of dorsal bay behind RSO]
│   ├── Left_Chine_TEOC_Camera     [Explode: -2.0m X, -0.8m Z]
│   ├── Right_Chine_TEOC_Camera    [Explode: +2.0m X, -0.8m Z]
│   └── Forward_Chine_Upper_Skins  [Explode: ±2.5m X, +1.5m Z]
├── 04_Fuselage_JP7_Fuel_System
│   └── Tanks_01_Through_06A       [6 translucent amber/gold JP-7 heat-sink volumes + manifold]
├── 05_Fuselage_Titanium_Skeleton
│   ├── Ring_Bulkheads_FS295_FS1260 [Stays anchored on core datum with FS715 carry-through]
│   ├── Dorsal_Spine_Skin_Panels   [Explode: +3.2m Z]
│   └── Ventral_Belly_Skin_Panels  [Explode: -2.4m Z]
├── 06_Inner_And_Outer_Wings
│   ├── Wing_Titanium_Spar_Grid    [Stays anchored]
│   ├── Upper_Corrugated_Wing_Skin [Explode: +2.0m Z, ±1.5m X]
│   ├── Lower_Corrugated_Wing_Skin [Explode: -1.8m Z, ±1.5m X]
│   └── Composite_Sawtooth_Edges   [Explode: ±2.8m X outward]
├── 07_Left_Propulsion_Pod (Mirror for 08_Right_Propulsion_Pod at X = ±4.115m)
│   ├── Translating_Inlet_Spike    [Explode: -4.5m forward along nacelle axis + actuator shaft]
│   ├── Forward_Bypass_Cowl_Ring   [Explode: -2.2m forward]
│   ├── Nacelle_Upper_Cowl_Half    [Explode: +2.6m Z, -2.2m X]
│   ├── Nacelle_Lower_Cowl_Half    [Explode: -2.6m Z, -2.2m X]
│   ├── PW_J58_Core_And_6_Bypass   [Stays visible in mid-air or slides +2.5m aft]
│   └── Ejector_Nozzle_BlowIn_Ring [Explode: +4.2m aft]
├── 09_Flight_Control_Surfaces
│   ├── Twin_AllMoving_Rudders     [Explode: +2.8m Z along 15° inward cant axis]
│   └── Inboard_Outboard_Elevons   [Explode: +2.0m aft]
└── 10_Landing_Gear_Assemblies
    ├── Nose_Gear_Twin_Wheel       [Explode: -2.2m Z downward]
    └── Main_Gear_3Wheel_Bogies_LR [Explode: -2.2m Z downward, Silver Al-tires]
```
