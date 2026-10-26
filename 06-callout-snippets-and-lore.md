# Section 06: Interactive Callout Snippets & Phase-2 Engineering Metadata
## Ready-to-Use Inspection Cards for Interactive Model Examination (Claude / Astro / Blender Viewer)

> **Purpose:** In Phase 2 of your pipeline, examining or clicking parts of the exploded 3D SR-71A model triggers contextual engineering callouts and background history. Every snippet below is grounded in verified NASA Dryden, USAF Museum, and `T.O. 1SR-71A-1` data and mapped directly to the Blender collection names in [05-inner-workings-cutaways-exploded-rig.md](05-inner-workings-cutaways-exploded-rig.md).

---

## Hotspot Callout Cards (`12` Core Subsystems)

### 1. Airframe Titanium Skin & Chordwise Corrugations (`06_Inner_And_Outer_Wings`)
* **Headline:** `85%` Beta-Titanium Airframe Built to Grow in Flight
* **Operating Temp:** `450 °F – 600 °F` (`232 °C – 316 °C`) average skin; `950 °F+` (`510 °C+`) at leading edges & exhaust
* **Snippet:** At sustained `Mach 3.2` cruise, aerodynamic friction heats the airframe beyond the structural softening point of aluminum. Lockheed Skunk Works fabricated `85%` of the structure from titanium alloys (`Ti-13V-11Cr-3Al`). Because the aircraft expands several inches in flight, wing skins are stamped with chordwise corrugations acting as thermal expansion joints—causing fuel panels to seep JP-7 on the ground until supersonic heat seals the airframe tight.

### 2. Translating Axisymmetric Inlet Spike (`Translating_Inlet_Spike`)
* **Headline:** Computer-Controlled Shockwave Trap (`54%` of Total Thrust!)
* **Travel Distance:** `26 inches` (`0.66 m`) axial translation (`Mach 1.6` → `Mach 3.2+`)
* **Snippet:** Above `Mach 2.5`, the inlet nacelles generate **more propulsive thrust than the rotating turbojet core itself** (`~54%` inlet pressure recovery vs. `~17.6%` turbojet core and `~28.4%` afterburner/ejector). Starting at `Mach 1.6`, the conical spike retracts aft `1.625 inches` per `0.1 Mach` (up to `26 inches`), capturing the supersonic shockwave inside the throat and decelerating air from `Mach 3.2` to subsonic `Mach 0.4` inches ahead of the compressor face.

### 3. Pratt & Whitney J58 (`JT11D-20`) Continuous Bleed-Bypass Turboramjet (`PW_J58_Core_And_6_Bypass`)
* **Headline:** Hybrid Turbojet-Assisted Ramjet (`32,500 lbf` Thrust Each)
* **Signature Feature:** `6` External 4th-Stage Bleed-Bypass Ducts + `TEB` Chemical Ignition
* **Snippet:** At `Mach 3+`, inlet compression heats incoming air to `800 °F` (`427 °C`) *before* entering the compressor. Pratt & Whitney solved this by opening bleed valves behind the 4th compressor stage, routing `~20%` of compressed air through **six large external pipes** directly into the afterburner. Each engine carries a sealed tank of pyrophoric **Triethylborane (TEB)**—enough for `16` injections—which bursts into green flame on contact with air to ignite low-volatility JP-7 fuel.

### 4. JP-7 Fuel & Thermal Heat-Sink Architecture (`04_Fuselage_JP7_Fuel_System`)
* **Headline:** Fuel as Coolant, Hydraulic Actuator Fluid & CG Trim (`~80,000 lb` Capacity)
* **Flash Point:** `140 °F` (`60 °C`) — Extinguishes an open match at room temperature
* **Snippet:** Stored across **six large fuselage tanks (`1` through `6A`)** and inner-wing integral structures (with **zero fuel in the outer wings**), `JP-7` serves as the aircraft's primary **heat sink**—cooling the cockpits, avionics, hydraulic oil, and engine oil before burning at `300 °F` in the engines, while automated longitudinal transfer shifts Center of Gravity aft at Mach 3 to cut trim drag.

### 5. Free-Floating Blow-In Door Ejector Nozzle (`Ejector_Nozzle_BlowIn_Ring`)
* **Headline:** Variable Aerodynamic Exhaust Nozzle (`28.4%` of Cruise Thrust)
* **Snippet:** Surrounding the J58 afterburner exit is a ring of free-floating tertiary **"blow-in" doors** and segmented variable-area ejector flaps. At low speeds, ambient air is drawn inward through the open doors to cushion the exhaust stream; at `Mach 3.2` (`80,000+ ft`), the doors seal shut and the outer petals open wide so the supersonic plume expands across the full nacelle diameter.

### 6. Forward Cockpit — Pilot Station (`Pilot_RSO_Tub_And_Panels`)
* **Headline:** Mach 3.2 Flight Deck & Quartz V-Windscreen (`640 °F` Exterior)
* **Snippet:** Wearing a `David Clark S1030` full-pressure suit, the pilot monitors supersonic inlet stability via the **Triple Display Indicator (`KEAS` / `Mach` / `Altitude`)** and dual **Inlet Spike / Forward Bypass** gauges. An **Inlet Unstart**—when the shockwave pops out of a nacelle—triggers violent yaw in milliseconds, countered automatically by the Digital Automatic Flight and Inlet Control System (`DAFICS`).

### 7. Rear Cockpit — Reconnaissance Systems Officer (`RSO`) (`Pilot_RSO_Tub_And_Panels`)
* **Headline:** Sensor Command, Electronic Warfare & Navigation Brain
* **Snippet:** Operating behind two small side windows and an optical belly viewfinder, the RSO manages the mission route, `ANS` star-tracker, Defensive Electronic Countermeasures (`DEF`), Side-Looking Radar (`ASARS-1`), Optical Bar Camera (`OBC`), and `TEOC` chine cameras—capable of imaging **100,000 square miles per hour** from `85,000 feet`.

### 8. Nortronics `NAS-14V2` Astro-Inertial Navigation System (`Nortronics_ANS_StarTracker`)
* **Headline:** `"R2-D2"` Daylight Star-Tracker Behind the RSO
* **Snippet:** Mounted aft of the RSO bulkhead beneath a circular optical quartz dorsal window, `"R2-D2"` tracks up to `61` stars **in broad daylight** using a blue-light telescope on a gyro-stabilized platform, maintaining navigation accuracy within `~300 ft` across intercontinental Mach 3 sorties without GPS or radio emissions.

### 9. Blended Forward Chines & Radar-Absorbing Sawtooth Composites (`03_Avionics_And_Chine_Bays`)
* **Headline:** First Operational Low-Observable Shaping + Supersonic Vortex Lift
* **Snippet:** Comprising `15%` of the airframe via triangular phenyl-silane radar-absorbing composite tiles, the sharp lateral **"cobra hood" chines** reduce radar return while generating powerful leading-edge vortices over the inner delta wing to balance supersonic lift and house interchangeable `TEOC` cameras.

### 10. Detachable Modular Nose Bay (`01_Nose_Recon_Module`)
* **Headline:** Swappable `OBC` Panoramic Camera or `ASARS-1` Synthetic Aperture Radar
* **Snippet:** Forward of `FS 295`, the entire nose cone unbolts as a self-contained mission pod—configured either with the **Itek Optical Bar Camera** (`10,500 ft` of panoramic film scanning horizon-to-horizon) or **all-weather Synthetic Aperture Radar** looking `100+ miles` laterally into contested territory.

### 11. Twin `15°` Inward-Canted All-Moving Rudders (`Twin_AllMoving_Rudders`)
* **Headline:** Full-Fin Aerodynamic Rudders Pivoting Atop the Nacelles
* **Snippet:** Each entire vertical fin above the nacelle stub pivots as an **all-moving control surface**, canted `15°` inward to lower radar cross-section and provide instantaneous yaw authority during asymmetric Mach 3 inlet unstarts.

### 12. Aluminum-Impregnated Silver Main Landing Gear (`Main_Gear_3Wheel_Bogies_LR`)
* **Headline:** `22-Ply` Metallic Silver Tires Pressurized with Nitrogen (`415 psi`)
* **Snippet:** Three custom **B.F. Goodrich aluminum-powder-impregnated tires** per main bogie reflect conductive heat inside the `550 °F` wheel wells and support `140,000 lb` gross weights and `175+ knot` landings assisted by a `40-foot` dorsal drag chute.
