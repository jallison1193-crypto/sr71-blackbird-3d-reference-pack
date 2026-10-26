# Section 02: 3D Scans, Photogrammetry, Open-Source Meshes & Sub-Assemblies
## Downloadable & Inspectable 3D References for Blender MCP

> **Important Museum Scan Status Note (Verified Oct 2026):** Neither NASA's `nasa3d.arc.nasa.gov` repository nor the Smithsonian `3d.si.edu` portal currently publishes an official downloadable 3D mesh of the SR-71A (Smithsonian's Udvar-Hazy SR-71 record `nasm_A19920072000` is 2D media only). However, **museum photogrammetry captures** (IWM Duxford `61-7962`, Museum of Flight Seattle `J58` RealityCapture scan, and San Diego Polycam LiDAR capture) plus **open-source articulated CAD/AC3D sub-assemblies** are publicly available and cataloged below.

---

## 1. Photogrammetry & LiDAR Scans (Real Museum Hardware)

| Asset / Museum Subject | Type & Polycount | License / Download | Direct URL & Blender Usage |
| :--- | :--- | :--- | :--- |
| **SR-71A Blackbird `61-7962` — American Air Museum, IWM Duxford** (`mgg8`) | Museum-preserved SR-71A 3D mesh (`186,323` tris / `88,455` verts) with embedded textures, twin nacelles, inlet spikes & red markings | **CC0 1.0 Public Domain — Downloadable** (`.glb` / `.gltf` / `.usdz`) | **Viewer & Download:** https://sketchfab.com/3d-models/sr-71a-blackbird-61-7962-duxford-00c24dd3549a4f429dd1a0a2469e9ba4 <br>**Preview Thumb:** https://media.sketchfab.com/models/00c24dd3549a4f429dd1a0a2469e9ba4/thumbnails/41f0dd0c10864649a5a2294c7d089e47/fac607f2428642fd8663529633afb193.jpeg <br>*Use as primary 1:1 proportion & chine-curvature ground-truth overlay in Blender.* |
| **GRADD Pratt & Whitney J58 Engine Photogrammetry Scan — Museum of Flight, Seattle** (`gradd`) | **199-photo RealityCapture photogrammetry scan** (`2,499,747` tris / `1,249,760` verts) of an actual bare J58 (`JT11D-20`) turbojet | Inspectable 3D WebGL Photogrammetry Reference (Editorial) | **3D Scan Viewer:** https://sketchfab.com/3d-models/gradd-sr-71-blackbird-a12-j58-engine-3d-model-9fe852b2c84b442bb112aec9c8c8b29e <br>**Preview Thumb:** https://media.sketchfab.com/models/9fe852b2c84b442bb112aec9c8c8b29e/thumbnails/c6c3c3accc1a47d49e30517e0f7d2fa8/777ab3c94aee4ad099274c5a7056d34a.jpeg <br>*Essential 360° spatial ground-truth for plumbing, 6 external bleed-bypass tubes, fuel manifold, and afterburner cans.* |
| **Lockheed SR-71 Blackbird LiDAR / Photogrammetry Capture — San Diego Air & Space Museum (`A-12 / Blackbird`)** (`mdeetjen`) | Polycam Object-Mode LiDAR + photogrammetry spatial capture | Public Polycam 3D Capture | **3D Capture Viewer:** https://poly.cam/capture/02BE69A5-AED5-43CF-8536-8B8435C541CF <br>*Useful for checking forward chine cross-sections and ground stance.* |

---

## 2. Open-Source Articulated Aircraft & Cockpit Instrument Meshes (Direct Git Clone / Download)

### A. `FGMEMBERS/Lockheed-SR71` (GPL-2.0 — Complete Articulated AC3D `.ac` + XML Hierarchy)
* **GitHub Repository:** https://github.com/FGMEMBERS/Lockheed-SR71
* **Author:** Emmanuel Baranger (`helijah`)
* **Total 3D/Texture/Rig Files:** `104` files (`Models/*.ac` ASCII AC3D meshes—directly readable by Python or Blender AC3D importer—plus XML pivot/axis definitions and `.png` gauge textures).
* **Why This Is Gold for Blender MCP:**
  * Contains **separated, named sub-meshes and exact pivot coordinates** in XML for control surfaces (inboard/outboard elevons, twin rudders, landing gear struts/doors, canopy) AND **13 individual 3D cockpit instruments**:
    * Attitude Indicator: `Models/Interior/Panel/Instruments/ai/ai.ac`
    * Altimeter: `Models/Interior/Panel/Instruments/altimeter/altimeter.ac`
    * Clock: `Models/Interior/Panel/Instruments/clock/clock.ac`
    * Dual EGT Gauges: `Models/Interior/Panel/Instruments/egt/egt.ac`
    * Fuel Quantity / Flow: `Models/Interior/Panel/Instruments/fuel/fuel.ac`
    * Horizontal Situation Indicator (HSI): `Models/Interior/Panel/Instruments/hsi/hsi.ac`
    * Mach / KEAS Indicator: `Models/Interior/Panel/Instruments/mach/mach.ac`
    * Magnetic Compass: `Models/Interior/Panel/Instruments/mag-compass/mag-compass.ac`
    * Oil Pressure & Oil Temp: `Models/Interior/Panel/Instruments/oilpressure/oilpressure.ac`, `oiltemp/oiltemp.ac`
    * Radar / RSO Scope: `Models/Interior/Panel/Instruments/radar/radar.ac`
    * Dual Tachometer (`% RPM`): `Models/Interior/Panel/Instruments/rpm/rpm.ac`
    * Airspeed Indicator: `Models/Interior/Panel/Instruments/speed/speed.ac`
* **Also Downloadable as `.glb`/`.gltf` on Sketchfab (`helijah`):**
  * https://sketchfab.com/3d-models/lockheed-sr-71-blackbird-1850c7bb7ac54902bd9868381ff8b652 (`69,135` faces, `42,423` verts, Free Standard Download).

---

## 3. Downloadable J58 Engine & Full Airframe Base Meshes (Sketchfab)

| Model Name | Polycount | License & Download | URL & Best Use |
| :--- | :--- | :--- | :--- |
| **Pratt & Whitney J58 Jet Engine** (`amadeussvx`) | `262,638` faces / `138,889` verts | **Downloadable** (`CC BY-NC-SA`) | https://sketchfab.com/3d-models/j58-jet-engine-bca3015516304cfabe249cfad5363939 <br>**Thumb:** https://media.sketchfab.com/models/bca3015516304cfabe249cfad5363939/thumbnails/dcc78a18d50e49b181d24f767ed5d2ac/34b5c769eb2a4761b70e890dc71c4095.jpeg <br>*High-poly standalone J58 turbojet + bypass tubes + afterburner—ideal starting reference for the internal engine bay!* |
| **SR-71 J58 Engine with Afterburner** (`BSODGamer1234`) | `1,120` faces / `566` verts | **Downloadable** (`CC BY`) | https://sketchfab.com/3d-models/sr-71-j58-engine-with-afterburner-8db0acd1e2624e168581887804801b2f <br>*Lightweight blockout proxy for testing exploded-view translation tracks.* |
| **Lockheed SR-71 "Blackbird"** (`ioai25312`) | `49,063` faces / `26,524` verts | **Downloadable** (`CC BY`) | https://sketchfab.com/3d-models/lockheed-sr-71-blackbird-e2400e6119f5414c89e075654a82d30a <br>**Thumb:** https://media.sketchfab.com/models/e2400e6119f5414c89e075654a82d30a/thumbnails/290b1991e28d4b6982e51582a704cfa6/09d501ec9b144497a600345467f350ec.jpeg <br>*Clean mid-poly exterior airframe mesh.* |
| **Lockheed SR-71 Blackbird** (`Spark_Customs`) | `37,018` faces / `18,407` verts | **Downloadable** (`CC BY`) | https://sketchfab.com/3d-models/lockheed-sr-71-blackbird-9076a8fb5a4340a9b6e543a2e4728a9c <br>**Thumb:** https://media.sketchfab.com/models/9076a8fb5a4340a9b6e543a2e4728a9c/thumbnails/ea36941c652d4efb93b8327abf19d1e7/cc4a38f049c044029f08a9fa882e0cbc.jpeg |

---

## 4. Inspectable Structural / Rib-Frame & Cockpit Instrument 3D References

* **Skeletal Blackbird (SR-71) — Structural Rib/Spar Visualization (`sy-kim`, `5.3M` tris):**
  * **Graphite Edition:** https://sketchfab.com/3d-models/skeletal-blackbirdsr-71-graphite-32a822fb0eab4cd6a73fc839a8cbe998
  * **Skeleton Edition:** https://sketchfab.com/3d-models/skeletal-blackbirdsr-71-skeleton-ac3ed6faf9094ead90dabe22aceba2b7
  * **Preview Image:** https://media.sketchfab.com/models/ac3ed6faf9094ead90dabe22aceba2b7/thumbnails/7c17d4b20d5846d1a80e67805fc957d0/22448b0e473645398acd7732558e090b.jpeg
  * *Note:* Artistic/structural skeletal rib-and-bulkhead interpretation inside the exact SR-71 silhouette—excellent visual inspiration for modeling internal titanium ring-frames and wing spars when outer skin panels lift away in the exploded view.
* **High-Detail Individual SR-71 Cockpit Controls & Gauges (`Cesar.Ferrolho` — 3D WebGL Inspectable):**
  * **SR-71 Flightstick (Control Stick Grip, Trim Hat & Triggers):** https://sketchfab.com/3d-models/sr-71-flightstick-448d8f5727af4f05b1017f6e6fb33587 (`5,538` faces)
  * **SR-71 Triple Display Indicator — KEAS / Mach / Altitude (`TDI` v2 with conversion chart):** https://sketchfab.com/3d-models/sr-71-triple-display-indicator-second-version-da9d101f8c3844fe9da1f7cb5475e156 (`2,546` faces)
  * **SR-71 Main Attitude Indicator (ADI):** https://sketchfab.com/3d-models/sr-71-attitude-indicator-3f2883f756a24efc80eb984f6e7c0055 (`3,440` faces)
  * **SR-71 Altimeter:** https://sketchfab.com/3d-models/sr-71-altimeter-a548685b22e8446d9a8cb26ba341d3a7 (`1,900` faces)
  * **SR-71 Instantaneous Vertical Speed Indicator (IVSI):** https://sketchfab.com/3d-models/sr-71-ivsi-instrument-8ba481364e974877889d46d3c7235985 (`1,585` faces)
* **High-Poly Exterior Airframe Topology Reference (`iliedom`, `300,116` faces):**
  * https://sketchfab.com/3d-models/lockheed-sr-71a-blackbird-e8888c4342bd40b3b95af3c6fcb0f963
