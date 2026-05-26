# Recuperated Gas Turbine Car — Concept Design Specification

---

## Table of Contents

- [Historical Background — The Turbine Car Programmes](#historical-background)
1. [Recommended Engine](#1-recommended-engine)
2. [Output Shaft and Step-Down Gearbox](#2-output-shaft-and-step-down-gearbox)
3. [Mass Flow Rate](#3-mass-flow-rate)
4. [What the Heat Exchanger Does](#4-what-the-heat-exchanger-does)
5. [Recuperator Thermal Summary](#5-recuperator-thermal-summary)
6. [Heat Exchanger Specification](#6-heat-exchanger-specification)
7. [FOD Protection](#7-fod-protection)
8. [Electrical System](#8-electrical-system)
9. [Fuel Cell](#9-fuel-cell)
10. [Fuel Consumption and Range](#10-fuel-consumption-and-range)
11. [Summary Table](#11-summary-table)
12. [Alternative Engine — Lighter Vehicle Application](#12-alternative-engine--lighter-vehicle-application)
13. [Lower Power Option — 100 to 200 HP Range](#13-lower-power-option--100-to-200-hp-range)
14. [Acceleration Estimates — All Engines](#14-acceleration-estimates--all-engines)
15. [FADEC Derating — How Power Limiting Works](#15-fadec-derating--how-power-limiting-works)
16. [Time Between Overhaul (TBO)](#16-time-between-overhaul-tbo)
17. [Three-Engine Comparison Summary](#17-three-engine-comparison-summary)
18. [Compatible Fuels and Seal Materials](#18-compatible-fuels-and-seal-materials)
19. [Water Injection System](#19-water-injection-system)
20. [Air Movement — Volumetric Flow and Pressure Drop](#20-air-movement--volumetric-flow-and-pressure-drop)
21. [Heat Exchanger Plate Geometry — M250-C18](#21-heat-exchanger-plate-geometry--m250-c18)
22. [Ancillary Systems, Costs and Instrumentation](#22-ancillary-systems-costs-and-instrumentation)
23. [Turbine Operations — Startup, Shutdown, and Controls](#23-turbine-operations--startup-shutdown-and-controls)
24. [Sourcing the Fuel Control Lever, Relays, and Electrical Components](#24-sourcing-the-fuel-control-lever-relays-and-electrical-components)
25. [Suggested Livery and Markings](#25-suggested-livery-and-markings)
26. [Commercially Available and Serviceable Recuperator Options](#26-commercially-available-and-serviceable-recuperator-options)
27. [Exhaust Duct Calculations — All Three Engines](#27-exhaust-duct-calculations--all-three-engines)
28. [CFD and Simulation Tools for Heat Exchanger Analysis](#28-cfd-and-simulation-tools-for-heat-exchanger-analysis)
29. [Plate Pair Spacing — Calculated Values and Surface Enhancement](#29-plate-pair-spacing--calculated-values-and-surface-enhancement)
30. [Donor Vehicle Selection and ABS System](#30-donor-vehicle-selection-and-abs-system)
31. [Cruise Power and Real-World Fuel Consumption](#31-cruise-power-and-real-world-fuel-consumption)
32. [Reference Documents and Links](#32-reference-documents-and-links)
33. [Glossary](#33-glossary)

---

## Historical Background

### Why This Concept Has Deep Roots

The gas turbine car is not a new idea. It was pursued seriously and publicly by multiple major manufacturers across three decades — and came remarkably close to production. Understanding what was achieved, what failed, and why it failed is essential context for any modern revival of the concept.

---

### General Motors Firebird Series — 1953 to 1964

General Motors had been researching the potential of turbine engines since the 1940s, but it wasn't until the early 1950s that a completed real-life prototype emerged. The result was a series of four concept vehicles — the GM Firebird series — each more extreme than the last, built for the annual Motorama auto shows and never intended for public sale.

**Firebird I (XP-21) — 1953/1954**

The first gas turbine automobile ever built and tested in the United States. The Whirlfire Turbo-Power gas turbine engine produced 370 horsepower at 13,000 rpm, expelling exhaust at 677°C. Purely a test and show vehicle, never road-registered.

**Firebird II — 1956**

A GT-304 Whirlfire unit producing 200 HP in a four-seat family car concept, complete with titanium body and an early vision of automatic highway guidance.

**Firebird III — 1959**

A two-seater powered by a 225 HP Whirlfire GT-305 engine and a separate two-cylinder 10 HP gas engine to power accessories. Seven fins, bubble canopy, single joystick replacing the steering wheel.

**Firebird IV — 1964**

Non-functional pure styling exercise. Reportedly crushed in the 1980s.

None of the four Firebirds were ever intended for the road. The turbine technology was real; the cars were showmanship.

---

### Chrysler Turbine Car — The Real Public Test

Where GM used turbines for showmanship, Chrysler used them for science. Chrysler's turbine programme ran from the late 1930s through to 1979 — forty years of continuous engineering development across seven engine generations.

The fourth-generation A-831 engine powered the famous Ghia-bodied Turbine Car of the public loaner programme. From October 1963 to January 1966, 55 cars were distributed to 203 volunteers in 48 states free of charge for three months each, cumulatively covering more than one million miles.

**Fuel Consumption — The Honest Figures**

| Source | Reported economy |
|---|---|
| Average fleet figure (Chrysler records) | **13 mpg US (18.1 L/100km)** |
| Best reported (highway) | **18–19 mpg US (12.4–13.1 L/100km)** |
| Typical town driving | **14.5 mpg US (16.2 L/100km)** |
| Worst reported (enthusiastic driving) | **11–11.5 mpg US (20.5–21.4 L/100km)** |
| Contemporary V8 equivalent car | ~15 mpg US (15.7 L/100km) |

---

### What Killed the Programme — The 1970s Fuel and NOx Crisis

The Chrysler turbine programme did not die from engineering failure. It was killed by two external forces arriving simultaneously in the early 1970s: NOx regulations from the newly formed EPA, and the 1973 and 1979 oil crises which shifted public attention entirely to fuel economy.

Advances in Dry Low NOx (DLN) combustion technology have since lowered NOx emissions from the 150–300 ppm level of the 1980s to the 15–40 ppm level today — a 90% reduction. The concept was not wrong. The technology simply needed another fifty years.

---

### Technology Comparison — 1963 vs Modern

| Parameter | Chrysler A-831 (1963) | Modern M250-C18 recuperated | Improvement |
|---|---|---|---|
| Engine power | 130 HP | 250 HP continuous | — |
| Recuperator | Rotary regenerator | Fixed plate — no moving parts | More reliable |
| Recuperator effectiveness | ~91–97% | ~90% | Comparable |
| NOx (combustor type) | Diffusion flame — ~500+ ppm | Modern annular — 15–40 ppm | **~90–95% lower** |
| Throttle lag | Significant complaint | Much reduced — variable geometry | Improved |
| Cold start | Complicated procedure | FADEC automated | Greatly improved |
| Multi-fuel | Yes — diesel, petrol, kerosene | Yes — plus biodiesel, ethanol | Broader |

---

## 1. Recommended Engine

**Rolls-Royce M250-C47B**

| Parameter | Value |
|---|---|
| Certification date | ~2000 — within 10–15 year preference window |
| Maximum takeoff power | 650 SHP (485 kW) |
| Continuous derated power | 450–500 SHP (336–373 kW) |
| Engine control | FADEC — single channel electronic with hydromechanical manual backup |
| Configuration | Two-shaft free power turbine |
| Output shaft speed | 6,000 RPM |
| Pressure ratio | 9.2:1 |
| Airflow (mass flow) | 2.77 kg/s (6.1 lb/s) |
| Dry weight | ~72 kg |
| Construction | Modular — compressor, gearbox, turbine, combustion sections separable |

Running derated at 450–500 SHP provides substantial margin below the 650 SHP maximum, extending TBO significantly and reducing thermal stress on all hot-section components.

---

## 2. Output Shaft and Step-Down Gearbox

The M250-C47B internal gearbox delivers **6,000 RPM** at the output flange. A step-down reduction gearbox is required.

| Parameter | Value |
|---|---|
| Input speed | 6,000 RPM |
| Required output speed | 2,000–3,000 RPM |
| Reduction ratio | 2:1 to 3:1 |
| Power rating required | 500+ HP continuous |

Units from within the M250 helicopter ecosystem are an obvious source, already rated for this exact shaft speed and power level.

---

## 3. Mass Flow Rate

$$\dot{m} = \mathbf{2.77\ kg/s}$$

Confirmed published figure for the M250-C40/C47 family at pressure ratio 9.2:1. Both recuperator packages share this flow equally, each handling **1.385 kg/s**.

---

## 4. What the Heat Exchanger Does

The heat exchanger in this design is a **recuperator** — a static, counterflow, gas-to-gas plate heat exchanger with no moving parts. It performs five distinct functions simultaneously.

### Function 1 — Waste Heat Recovery (Primary Purpose)

A simple-cycle gas turbine exhausts gas at around **546°C** after the power turbine has extracted useful work. The recuperator captures this heat and transfers it to the cold compressed air before it enters the combustor. The result is a **~30% reduction in fuel consumption**. The recuperator is what makes the concept viable.

### Function 2 — Exhaust Cooling

The hot exhaust gas cools from ~546°C at the turbine exit to approximately **177–282°C** at the recuperator hot-side outlet. Without the recuperator the exhaust would exit at over 500°C — capable of igniting materials it contacts.

### Function 3 — Intake Air Preheating

Warmer air entering the combustor means a more stable, complete combustion process — lower CO and unburned hydrocarbon emissions, and more consistent combustion across the full power range.

### Function 4 — FOD Protection

The recuperator cold side acts as a natural **Foreign Object Damage (FOD) barrier**. The narrow plate channels physically prevent insects, leaves, grit, small stones, water droplets, and ice crystals from reaching the compressor. No separate **Inlet Particle Separator (IPS)** is required.

### Function 5 — Partial Exhaust Noise Attenuation

As exhaust gas passes through the narrow plate channels, acoustic energy is partially absorbed and dissipated. The recuperator acts as a partial muffler, reducing high-frequency turbine whine before the exhaust reaches the rear duct silencer.

### Summary of Recuperator Functions

| Function | Benefit |
|---|---|
| Waste heat recovery | ~30% fuel saving — makes the concept viable |
| Exhaust cooling | Reduces outlet temperature from ~546°C to ~177–282°C |
| Intake air preheating | Cleaner combustion, lower emissions on biodiesel |
| FOD protection | Eliminates need for separate inlet particle separator |
| Partial noise attenuation | Reduces turbine whine before rear silencer |

---

## 5. Recuperator Thermal Summary

### Cycle State Point Temperatures

| Parameter | +5°C ambient | +20°C ambient | +45°C ambient |
|---|---|---|---|
| Compressor inlet T1 | 278 K (5°C) | 293 K (20°C) | 318 K (45°C) |
| Compressor outlet T2 — cold side IN | 605 K (332°C) | 638 K (365°C) | 692 K (419°C) |
| Turbine exhaust T4 — hot side IN | 819 K (546°C) | 819 K (546°C) | 819 K (546°C) |
| Preheated air T3 — cold side OUT | 814 K (541°C) | 819 K (546°C) | 806 K (533°C) |
| **Final exhaust T5 — hot side OUT** | **610 K (337°C)** | **638 K (365°C)** | **705 K (432°C)** |
| Recuperator heat duty | 582 kW | 504 kW | 318 kW |

The design case for maximum heat duty is the **+5°C cool start scenario** at **582 kW**.

---

## 6. Heat Exchanger Specification

### Design Basis

| Parameter | Value |
|---|---|
| Recuperator effectiveness (ε) | 0.90 (90%) |
| NTU (Number of Transfer Units) | 9.0 |
| Overall heat transfer coefficient (U) | 100 W/m²K (enhanced plate surface) |
| LMTD at design condition | 5°C (counterflow, high effectiveness) |
| Design heat duty | 582 kW at +5°C ambient |

### Split Configuration — Two Packages

| Parameter | Per Package | Total |
|---|---|---|
| Base surface area | 582 m² | 1,164 m² |
| **Primary surface area (+20%)** | **698 m²** | **1,397 m²** |
| Core volume (est.) | ~0.82 m³ | ~1.64 m³ |
| Physical envelope (approx.) | 650 × 540 × 230 mm | — |
| Mass flow handled | 1.385 kg/s | 2.77 kg/s |

### Construction

| Parameter | Specification |
|---|---|
| Plate geometry | Dimple/bump enhanced primary surface — not corrugated |
| Flow arrangement | Counterflow |
| Joining method | Vacuum brazed |
| Material | SS347 stainless steel |
| Material temperature limit | ~675°C sustained — adequate throughout |
| Hot side inlet temperature | 546°C — within SS347 capability with margin |

---

## 7. FOD Protection

Fresh combustion air is drawn through the cold side of the recuperator before reaching the compressor inlet. The narrow plate channels act as an effective barrier against debris.

**No separate Inlet Particle Separator (IPS) is required.** A simple weather-proof intake scoop with a coarse mesh screen upstream of the recuperator cold side inlet is sufficient.

---

## 8. Electrical System

Two 12V / 600A AGM batteries connected in series providing 24V for engine startup.

| Function | Supply |
|---|---|
| Engine startup | 24V across both batteries in series |
| Car electronics (lights, instruments etc.) | 12V tapped at Battery 1 positive to ground |
| Battery charging (running) | Starter-generator 28V charges both batteries in series — each sees ~14V |

No relay, no DC-DC converter, no switching logic required.

---

## 9. Fuel Cell

### Available Options — ATL Saver Cell Series

| Capacity | Approximate Dimensions (with aluminium container) | Notes |
|---|---|---|
| 100 litres | 671 × 671 × 340 mm (low profile) | Readily available, standard stock item |
| 120 litres | 641 × 465 × 420 mm | Standard stock item |
| 120 litres | 620 × 416 × 535 mm | FIA approved alternative profile |

**Recommended: ATL 120 litre Saver Cell** — maximum within the stated 130-litre limit, FIA FT3-1999 approved, biodiesel compatible with blue foam baffle specification.

---

## 10. Fuel Consumption and Range

### SFC Basis

The confirmed published SFC for the M250-C47B at cruise power is **0.65 lb/SHP/hr**. Running derated at **450 SHP continuous:**

$$\text{Recuperated fuel flow} = 150.8 \times 0.70 = \mathbf{106\ \text{litres/hr}}$$

### Running Time and Range

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **28 minutes** | **~39 km** |
| 100 litres | **57 minutes** | **~78 km** |
| **120 litres (recommended)** | **~68 minutes** | **~93 km** |
| Required for 165 km / 2 hrs | — | **~212 litres needed** |

---

## 11. Summary Table

| Parameter | Value |
|---|---|
| **Engine** | Rolls-Royce M250-C47B |
| **Maximum power** | 650 SHP |
| **Continuous derated power** | 450–500 SHP |
| **FADEC** | Yes — single channel + hydromechanical backup |
| **Output shaft speed** | 6,000 RPM |
| **Step-down gearbox** | Required — 2:1 to 3:1 reduction |
| **Mass flow rate** | **2.77 kg/s** |
| **Total recuperator surface area (base)** | **1,164 m²** |
| **Total recuperator surface area (+20%)** | **1,397 m²** |
| **Per package surface area (+20%)** | **698 m²** |
| **Per package envelope** | **650 × 540 × 230 mm** |
| **Intake duct diameter (per package)** | **481 mm** |
| **Recuperator material** | SS347 stainless steel |
| **Hot side inlet temperature** | 546°C |
| **Final exhaust temperature** | 337°C (design case +5°C ambient) |
| **Fuel** | Biodiesel (B100) |
| **Fuel cell** | ATL 120L Saver Cell — 641 × 465 × 420 mm |
| **Recuperated fuel flow** | ~106 litres/hr at 450 SHP |
| **Range on 120 litres** | **~93 km / ~68 minutes** |
| **Electrical startup** | 24V — 2 × 12V / 600A AGM batteries in series |
| **Car electronics supply** | 12V tapped at Battery 1 positive terminal to ground |

---

## 12. Alternative Engine — Lighter Vehicle Application

### Rolls-Royce RR300

| Parameter | Value |
|---|---|
| Type | Twin-spool free-turbine turboshaft |
| Certification | February 2008 (FAA) |
| Maximum takeoff power | **300 SHP (224 kW)** |
| Maximum continuous power | **240 SHP (179 kW)** |
| Engine control | **FADEC** |
| Pressure ratio | **6.2:1** |
| Output shaft speed | ~6,000 RPM (M250 family standard) |
| Dry weight | **79.8 kg (176 lb)** |
| SFC at cruise | **0.63 lb/SHP/hr** |
| Airflow | ~1.87 kg/s (scaled from M250 family) |
| Primary application | Robinson R66 helicopter |

### RR300 Fuel Consumption and Range

Recuperated fuel flow at 210 SHP: **48 litres/hr**.

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **63 minutes** | **~86 km** |
| 100 litres | **125 minutes** | **~172 km** |
| **120 litres (ATL recommended)** | **~150 minutes (2hrs 30min)** | **~206 km** |

**The 120 litre ATL Saver Cell comfortably exceeds the 165 km / 2-hour target with the RR300.** This is the critical result.

### Comparative Summary — M250-C47B vs RR300

| Parameter | M250-C47B | RR300 | Advantage |
|---|---|---|---|
| Max power | 650 SHP | 300 SHP | C47B |
| Continuous derated | 450–500 SHP | 200–210 SHP | RR300 (right-sized) |
| Mass flow | 2.77 kg/s | ~1.87 kg/s | RR300 (smaller system) |
| Total HX surface area | 1,164 m² | **120 m²** | **RR300** |
| Hot side inlet temp | 546°C | **478°C** | **RR300** |
| Final exhaust temp (+5°C) | 337°C | **282°C** | **RR300** |
| Recuperated fuel flow | 106 litres/hr | **48 litres/hr** | **RR300** |
| Range on 120 litres | ~93 km | **~206 km** | **RR300** |
| Meets 165 km target? | **No** (needs ~212L) | **Yes** (120L — margin to spare) | **RR300** |

### Conclusion

**The Rolls-Royce RR300 is the correct engine for this concept** for a 1,200–1,500 kg vehicle.

---

## 13. Lower Power Option — 100 to 200 HP Range

### Recommended Engine: Rolls-Royce M250-C18

The original JetRanger engine — the engine that started the M250 family in 1960. By far the most produced small turboshaft in history.

| Parameter | Value |
|---|---|
| Type | Two-shaft free-turbine turboshaft |
| Certification | 1960s — extremely mature |
| Maximum takeoff power | **317 SHP (236 kW)** |
| Maximum continuous power | **250 SHP (186 kW)** |
| Pressure ratio | **6.2:1** |
| Airflow | **1.23 kg/s** |
| SFC | **0.64 lb/SHP/hr** |
| Output shaft speed | **6,000 RPM** |
| Dry weight | **64 kg (141 lb)** |
| Engine control | Hydromechanical (Honeywell/Bendix FCU) |
| Applications | Bell 206 JetRanger, Hughes 500, MD500 |
| Units produced | 38,000+ (M250 family total) |

### M250-C18 Fuel Consumption and Range

Recuperated fuel flow at 220 SHP: **51 litres/hr**.

| Fuel cell | Running time | Range at 82.5 km/hr |
|---|---|---|
| 50 litres | **59 minutes** | **~81 km** |
| 100 litres | **118 minutes (1hr 58min)** | **~162 km** |
| **120 litres** | **~141 minutes (2hrs 21min)** | **~194 km** |

The 120 litre cell comfortably exceeds the 165 km target.

---

## 14. Acceleration Estimates — All Engines

Vehicle mass: **1,500 kg**. Rear tyre width: **200 mm**, μ = 1.20 on dry tarmac. Drivetrain efficiency: **η = 0.88**. Maximum traction-limited acceleration: **5.30 m/s² (0.54g)**.

| Engine | Max power | 0–100 km/h | Character |
|---|---|---|---|
| M250-C47B | 650 SHP | **~5.2 s** | Traction-limited throughout — tyre-shredding potential |
| RR300 | 300 SHP | **~5.2 s** | Near-identical feel to C47B below 100 km/h |
| **M250-C18** | **317 SHP** | **~5.7 s** | 0.5 s slower — still very brisk, most practical |

---

## 15. FADEC Derating — How Power Limiting Works

Running a turbine below its certificated maximum power extends component life dramatically. Reducing TGT by as little as 25°C can double hot-section life.

### The Four Primary Limits

**1. TGT Limit (Turbine Gas Temperature)** — the most important limit for hot-section life.

**2. NG Limit (Gas Generator Speed)** — lowering the NG ceiling reduces compressor delivery pressure and temperature.

**3. Torque Limit (Q)** — the most practically useful limit for a car application. Protects the step-down gearbox and drivetrain.

**4. NP Limit (Power Turbine Speed)** — power turbine overspeed protection.

### Dual-Mode Calibration for This Car

**Touring mode** — TGT limit reduced by 40–50°C below maximum, torque limit set to approximately 70% of peak. Normal everyday driving.

**Performance mode** — Full certificated limits restored. Used for overtaking, hill climbing, or track use. Time at this power level is logged by the FADEC health monitoring system.

### FADEC Interface and Pinout Documentation

The M250-C47B FADEC uses a **MIL-DTL-38999 Series III** circular connector. The maintenance port uses an **RS-422 serial interface** at 19,200 baud for fault code reading via the Rolls-Royce **CEDAM** software.

---

## 16. Time Between Overhaul (TBO)

| Engine | Component | TBO | Years at 200 hrs/yr |
|---|---|---|---|
| M250-C18 (Series II) | Compressor + Turbine | **3,500 hours** | **~17 years** |
| RR300 | Engine (all modules) | **2,000 hours** | **~10 years** |
| M250-C47B (Series IV) | Turbine | **2,000 hours** | **~10 years** |

Running derated in touring mode with TGT reduced by 40–50°C, every 15°C reduction doubles creep life. A 45°C reduction multiplies blade life by approximately **8×**.

---

## 17. Three-Engine Comparison Summary

| Parameter | M250-C47B | RR300 | M250-C18 |
|---|---|---|---|
| Max power | 650 SHP | 300 SHP | 317 SHP |
| Continuous power | 450–500 SHP | 240 SHP | 250 SHP |
| Mass flow | 2.77 kg/s | ~1.87 kg/s | **1.23 kg/s** |
| Pressure ratio | 9.2:1 | 6.2:1 | 6.2:1 |
| **HX area +20% (total)** | **1,397 m²** | **143 m²** | **64 m²** |
| Per package HX envelope | 650×540×230 mm | 320×270×100 mm | **615×430×389 mm** |
| Engine weight | ~72 kg | ~80 kg | **64 kg** |
| FADEC | Yes | Yes | No (see §15) |
| TBO — turbine | 2,000 hrs | 2,000 hrs | **3,500 hrs** |
| Recuperated fuel flow | 106 L/hr | 48 L/hr | **51 L/hr** |
| Range on 120L | ~93 km | ~206 km | **~194 km** |
| 0–100 km/h | ~5.2 s | ~5.2 s | ~5.7 s |
| Support network | Excellent | Excellent | **Best of all** |
| Relative cost | High | Medium | **Lowest** |
| Best suited for | Performance showcase | Balanced touring | Practical daily use |

---

## 18. Compatible Fuels and Seal Materials

### Table A — Liquid Fuel Candidates

| Fuel | NOx vs Diesel | Seal Risk | Notes |
|---|---|---|---|
| **Biodiesel B100** | Slightly lower | Medium — FKM preferred | Best balance of NOx, energy density and range. **Recommended primary fuel** |
| **HVO** (Hydrotreated vegetable oil) | Similar to diesel | Low — standard seals acceptable | Excellent cold weather performance |
| **Bio-ethanol 80%** | Much lower | High — FKM required | Best NOx. ~1.6× fuel flow |
| **Bio-methanol** | Lower | Very high — FKM + PTFE essential | Toxic — handling precautions needed |
| **Jet A-1 / kerosene** | Baseline | Low — standard seals | Very wide availability |
| **Diesel (EN590)** | Baseline | Low — standard seals | Widely available |
| **Leaded petrol (100LL Avgas)** | — | — | **AVOID — lead destroys turbine nozzle guide vanes irreversibly** |

### Table B — Seal Material Compatibility

Specify **FKM (Viton) for all O-rings and dynamic seals**, **PTFE-lined hose throughout**, and **stainless steel fittings**. Standard NBR (nitrile) seals degrade rapidly in biodiesel and alcohols — do not use.

---

## 19. Water Injection System

Water injection serves two simultaneous roles: NOx reduction at all power levels, and power augmentation on demand.

| Parameter | Value |
|---|---|
| Water source | Rainwater from household downspout |
| Storage tank | 15–25 litres — stainless or HDPE |
| Operating pressure | 70–100 bar |
| Pump control | **PWM — duty cycle proportional to throttle position** |
| Droplet size | <20 micron — complete evaporation before compressor |
| Injection point | Upstream of recuperator cold side inlet |
| Cruise injection rate | 0.3–1.0 L/min |
| Full power injection rate | 4.0–5.0 L/min |
| NOx effect | 20–35% reduction at cruise rates |
| Power augmentation | 10–15% additional shaft power at full rate |

| Throttle position | PWM duty cycle | Injection rate | Effect |
|---|---|---|---|
| Idle | 0% | Off | No injection |
| Light cruise | 10–20% | ~0.3–0.5 L/min | Mild NOx reduction |
| Normal cruise | 20–40% | ~0.5–1.0 L/min | Steady NOx reduction |
| Hard acceleration | 60–80% | ~2.0–3.0 L/min | NOx reduction + power augmentation |
| Full throttle | 100% | ~4.0–5.0 L/min | Maximum augmentation |

---

## 20. Air Movement — Volumetric Flow and Pressure Drop

| Parameter | M250-C47B | RR300 | M250-C18 |
|---|---|---|---|
| Mass flow | 2.77 kg/s | 1.87 kg/s | 1.23 kg/s |
| **Intake volumetric flow (+5°C)** | **2.18 m³/s** | **1.47 m³/s** | **0.97 m³/s** |
| Cold side volumetric flow (pressurised) | 0.543 m³/s | 0.402 m³/s | 0.265 m³/s |
| **Hot side vol flow at T4 (turbine exit)** | **6.20 m³/s** | **3.84 m³/s** | **2.53 m³/s** |
| **Final exhaust vol flow at T5 (tailpipe)** | **4.62 m³/s** | **2.84 m³/s** | **1.87 m³/s** |
| Max total pressure drop (5% rule) | 46.6 kPa | 31.4 kPa | 31.4 kPa |
| Single tailpipe diameter — 20 m/s | 542 mm | 425 mm | 345 mm |
| Twin tailpipes each — 20 m/s | 383 mm | 300 mm | 244 mm |
| Hot duct per package — 15 m/s | 513 mm | 404 mm | 327 mm |

Every 1% of compressor delivery pressure lost to recuperator pressure drop reduces cycle thermal efficiency by approximately **0.3–0.5 percentage points**. Staying within 5% total is critical.

---

## 21. Heat Exchanger Plate Geometry — M250-C18

| Parameter | Value |
|---|---|
| **Plate height** | **430 mm** |
| **Plate length** | **615 mm** |
| **Plate thickness** | **0.10 mm SS347 foil** |
| **Ridge orientation** | Longitudinal — parallel to flow |
| **Cold side ridge height** | **1.5 mm** |
| **Hot side ridge height** | **5.0 mm** |
| **Ridge pitch** | **20 mm centre to centre** |
| **Ridges per plate** | **21** |
| **Plates per package (+20%)** | **116** |
| **Plate pairs per package** | **58** |
| **Cell pitch** | **6.70 mm** |
| **Stack height** | **389 mm** |
| **Package envelope** | **615 × 430 × 389 mm** |
| **Area per package (+20%)** | **31.9 m²** |
| **Cold side channel velocity** | **4.0 m/s** |
| **Hot side channel velocity** | **10.6 m/s** |
| **Intake duct (rectangular)** | **430 × 188 mm** |
| **Intake duct (round equivalent)** | **321 mm diameter** |

---

## 22. Ancillary Systems, Costs and Instrumentation

### Power Steering — Electric Hydraulic Pump (EHPS)

**Recommended unit: Volvo S40/V50/C30 EHPS pump (2006–2012)**

| Parameter | Value |
|---|---|
| Supply voltage | **12V** from Battery 1 |
| Current draw | ~20–25A at full lock, ~5A at straight-ahead cruise |
| Approximate cost | **€80–150** for used OEM pump + **€60–100** for controller |

### Brake Booster — Hella UP30 Electric Vacuum Pump

| Parameter | Value |
|---|---|
| Application | **Standalone — sole vacuum source** |
| Rated voltage | **14.0V** |
| Current draw | **<15A** |
| Max vacuum | **≥86% of ambient** |
| Time to 50% vacuum | **≤3.5s** |
| Booster volume | **4.0 litres** |
| Pump operating life | **1,200 hours** |
| Approximate cost | **€80–150** |

### Turbine Engine Instrumentation

| Instrument | Parameter | Notes |
|---|---|---|
| TGT gauge | Turbine Gas Temperature | Self-powered — no external supply needed |
| N1 gauge | Gas generator speed (%) | Monitors compressor/gas generator speed |
| Torque gauge | Output shaft torque (%) | Primary power indicator |
| Oil pressure | Engine oil pressure | Critical — low oil pressure = immediate shutdown |
| Oil temperature | Engine oil temperature | Monitors lubrication health |
| Fuel flow | Litres per hour | Range management |
| Fuel level | Tank contents | Standard automotive sender in ATL cell |
| FADEC warning light | Fault indication | Wired to FADEC fault output |
| Water level | Injection tank | Low level warning |

**Approximate instrumentation cost: €500–1,500** for a complete analogue set from aviation surplus.

### Engine Cost — M250-C18

| Condition | Price range (USD) |
|---|---|
| Core / run-out | $5,000–15,000 |
| Serviceable — time continued | **$15,000–35,000** |
| Recently overhauled (SMOH) | $40,000–70,000 |

---

## 23. IMPORTANT! Turbine Operations — Startup, Shutdown, and Controls

A gas turbine engine is not operated like a piston engine. The majority of gas turbine failures occur during startup, not during cruise.

### The Three Phases of Every Turbine Start

**Phase 1 — Motoring (Cranking)**

The starter motor spins the gas generator from rest with no fuel admitted. This continues until N1 reaches 10–15%. Motoring without fuel first is not optional.

**Phase 2 — Light-Off and Acceleration**

At minimum motoring speed, the igniter fires and fuel is admitted. The engine must accelerate fast enough to avoid:
- **Hot start** — TGT rising faster than the engine can accelerate
- **Hung start** — engine lights but fails to accelerate past 30–50% N1
- **No-light** — igniter fires but no combustion occurs

**Phase 3 — Stabilisation and Idle**

N1 stabilises at ground idle (62–68%). A minimum **2-minute warm-up at idle** is required before any torque load is applied.

### FADEC Startup — M250-C47B and RR300

The FADEC manages the entire start sequence automatically once initiated. The operator's role is: confirm prerequisites, initiate start, and monitor. The FADEC does the rest, including automatic hot start abort protection.

### Non-FADEC Startup — M250-C18

The M250-C18 uses a **Bendix/Honeywell DP-L2 hydromechanical FCU**. The operator performs every step manually and must intervene immediately if a hot start, hung start, or no-light develops.

**M250-C18 Start Procedure:**
1. MASTER BAT — ON
2. AVIONICS — ON (confirm instruments)
3. FUEL VALVE — OPEN
4. FUEL PUMP — ON
5. FUEL CONTROL — confirm OFF
6. AVIONICS — OFF (protect from starter spike)
7. STARTER — ON (motor to 12–15% N1)
8. IGNITION — ON
9. FUEL CONTROL — IDLE (light-off)
10. AVIONICS — ON (monitor TGT and N1)
11. At 60% N1 — STARTER OFF
12. At 65–70% N1 — IGNITION OFF
13. Confirm oil pressure ≥ minimum within 30 seconds
14. Wait 2-minute warm-up
15. WATER INJ — AUTO
16. FUEL CONTROL — RUN

### Shutdown — Both Engine Types

1. Throttle to IDLE
2. Wait **3 minutes at idle** — mandatory cool-down
3. WATER INJ — OFF
4. FUEL CONTROL — OFF
5. FUEL PUMP — OFF (after N1 reaches zero)
6. FUEL VALVE — CLOSE
7. AVIONICS — OFF
8. MASTER BAT — OFF

### The Complete Switch and Control Set

| Switch | Function | Type |
|---|---|---|
| MASTER POWER | Connects battery system to main bus | Guarded rocker or key switch |
| AVIONICS BUS | Powers instruments and FADEC | Toggle — OFF during starter cranking peak |
| FUEL CONTROL | Primary engine run/stop | Lever with detents: OFF / IDLE / RUN |
| THROTTLE | Normal driving power control | Accelerator pedal + TPS sensor (0–5V) |
| STARTER | Energises starter-generator | Guarded spring-return (FADEC) or maintained (C18) |
| IGNITION | Powers ignition exciter | Toggle ON/OFF — manual on C18, FADEC-managed on C47B/RR300 |
| FUEL PUMP | Energises electric boost pump | Toggle with indicator light |
| FUEL SHUTOFF VALVE | Firewall emergency fuel cutoff | Guarded toggle or T-handle — CLOSE as emergency measure |
| FIRE HANDLE | Combined emergency shutdown | Red T-handle with shear wire — closes fuel valve + cuts pump |
| WATER INJ MODE | Enables injection system | Three-position rotary: OFF / AUTO / MANUAL |
| TOURING / PERF MODE | Selects FADEC calibration map (FADEC only) | Two-position toggle |
| MASTER WARNING RESET | Silences audible warning after FADEC alert | Momentary pushbutton |

---

## 24. Sourcing the Fuel Control Lever, Relays, and Electrical Components

### The Three-Position Fuel Control Lever

| Source | Type | Approx. cost | Notes |
|---|---|---|---|
| Cockpit Innovations / Skysales | Machined aluminium throttle quadrant, single lever | €80–180 | Adjustable friction and detents, push-pull Bowden cable output |
| Van's Aircraft (vansaircraft.com) | Mixture control quadrant lever | $45–95 | Functionally identical — OFF / IDLE / FULL RICH = OFF / IDLE / RUN |
| Used Bell 206 cockpit parts | Actual M250-C18 fuel control lever from service | $30–120 | Correct detents and feel; requires custom bracket |

### Relay Summary Table

| Relay | Function | Type | Rating | Approx. cost |
|---|---|---|---|---|
| **Battery Master Contactor** | Main battery bus isolation | Albright SW180 | 200A cont / 1,000A int | **€25–55** |
| **Starter Relay** | Starter motor circuit | Albright SW80 or heavy automotive solenoid | 80–500A intermittent | **€18–35** |
| **Fuel Pump Relay** | Electric boost pump | Bosch 40A cube relay | 40A | **€2–5** |
| **Fuel Valve Relay** | Firewall shutoff valve coil | Bosch 40A cube relay | 40A | **€2–5** |
| **Water Pump Relay** | Injection pump switching | Bosch 40A cube relay | 40A | **€2–5** |

Total relay hardware cost: approximately **€49–105**.

---

## 25. Suggested Livery and Markings

### Safety Stencils

| Stencil text | Location | Basis |
|---|---|---|
| **DANGER — HOT EXHAUST** | Rear bodywork, above and beside exhaust outlets | Standard helicopter tailpipe marking |
| **CAUTION — TURBINE EXHAUST** | Rear lower valance | Standard turbine ground vehicle marking |
| **NO STEP** | Any body surface not engineered for standing load | Standard airframe marking |
| **INTAKE** with arrow | At intake scoops | Identifies the air inlet |
| **FUEL** with fuel type identifier | At fuel filler | Include B100 or BIODIESEL below |
| **WATER** | At water injection filler | Distinguish from fuel |
| **MAX TEMP 300°C / 572°F** | Rear bodywork around exhaust zone | Advisory to ground crew and bystanders |

### Filler Cap Colour Coding

- 🟢 **FUEL** — BIODIESEL B100 — green cap
- 🔵 **WATER** — WATER INJECTION — blue cap
- 🟡 **OIL** — ENGINE OIL — yellow cap

### Kill Markings

Small silhouette of each defeated opponent stencilled on a consistent panel — typically the door below the window line — in a single contrasting colour. Side elevation, no detail, black or white fill only. Unsolicited victories only.

---

## 26. Commercially Available and Serviceable Recuperator Options

### The Matching Requirement — M250-C18

| Parameter | Requirement |
|---|---|
| Mass flow (both packages combined) | **1.23 kg/s** |
| Hot side inlet temperature | **478°C** |
| Hot side outlet temperature | **282°C** |
| Cold side inlet temperature | **260°C** |
| Cold side outlet temperature | **456°C** |
| Effectiveness (ε) | **0.90** |
| Material | SS347 stainless or equivalent |
| Configuration | Counterflow — split two packages |

### Option 1 — Turbec T100 / Ansaldo AE-T100 (Best Match)

The Turbec T100 is a 100 kWe recuperated microturbine in continuous commercial production since the early 2000s. The recuperator is built by Rekuperator Svenska AB (RSAB) using 0.10 mm SS347 foil.

| Parameter | T100 recuperator | M250-C18 requirement | Match |
|---|---|---|---|
| Hot side inlet | **650°C** | 478°C | ✓ Within rating |
| Hot side outlet | **270°C** | 282°C | ✓ Close match |
| Mass flow | **~0.8 kg/s** | 1.23 kg/s | Use two in parallel |
| Effectiveness | **~90%** | 90% | ✓ Exact |
| Plate material | **SS347 — 0.1 mm foil** | SS347 — 0.1 mm foil | ✓ Identical |

### Comparative Summary

| Option | Mass flow fit | Geometry | Est. cost (pair) | Lead time |
|---|---|---|---|---|
| T100 / AE-T100 (used) | ~130% — slightly oversized | Flat pack — ideal | **€6,000–30,000** | Immediate if stock found |
| T100 / AE-T100 (new spare) | ~130% — slightly oversized | Flat pack — ideal | **€4,000–16,000** | Weeks |
| RSAB custom | Exact | Flat pack — ideal | **€10,000–40,000** | Months |
| Capstone C30 (extract) | ~50% each — needs 3–4 | Annular — adaptation required | **€5,000–15,000** | Immediate |
| Heatric PCHE | Exact | Very compact block | **€30,000–100,000+** | Months |

**The Turbec T100 / Ansaldo AE-T100 recuperator is the most practical route.**

---

## 27. Exhaust Duct Calculations — All Three Engines

Design case: **+5°C ambient**. Velocity targets: hot duct 15–20 m/s; tailpipe 20–30 m/s; exit diffuser 10 m/s.

### M250-C18 — Consolidated Dimension Reference

| Duct section | Preferred config | Diameter | Circumference |
|---|---|---|---|
| Hot duct — per package | 327 mm @ 15 m/s | **327 mm** | **1,028 mm** |
| Tailpipe — per package | 244 mm @ 20 m/s | **244 mm** | **766 mm** |
| Exit diffuser — per package | 345 mm @ 10 m/s | **345 mm** | **1,083 mm** |
| Intake duct — per package | 321 mm round @ 6 m/s | **321 mm** | **1,007 mm** |

### M250-C47B — Hot Duct

| Configuration | Velocity | Diameter | Circumference |
|---|---|---|---|
| Single duct | 15 m/s | 726 mm | 2,281 mm |
| **Per package (×2)** | **15 m/s** | **513 mm** | **1,611 mm** |
| Twin tailpipes each | 20 m/s | 383 mm | 1,205 mm |

### RR300 — Hot Duct

| Configuration | Velocity | Diameter | Circumference |
|---|---|---|---|
| **Per package (×2)** | **15 m/s** | **404 mm** | **1,269 mm** |
| Twin tailpipes each | 20 m/s | 300 mm | 944 mm |

---

## 28. CFD and Simulation Tools for Heat Exchanger Analysis

The recuperator requires **Conjugate Heat Transfer (CHT)** simulation — simultaneously solving two fluid domains and the solid SS347 plate between them.

### Recommended Tool Stack — OpenFOAM + CfdOF

OpenFOAM's `chtMultiRegionFoam` solver handles this problem. CfdOF is a FreeCAD addon that wraps OpenFOAM behind a graphical interface, installed via the FreeCAD Addon Manager.

**Key simplification:** model only a **single representative plate pair** with periodic boundary conditions on the lateral faces. This validates U at a fraction of the computational cost of modelling the full 116-plate stack.

### Installation — Ubuntu/Debian Linux

```bash
# OpenFOAM
sudo sh -c "wget -q -O - https://dl.openfoam.com/add-debian-repo.sh | bash"
sudo apt install openfoam2406-default

# ParaView (post-processing)
sudo apt install paraview

# GMSH (meshing)
sudo apt install gmsh

# FreeCAD AppImage — download from https://github.com/FreeCAD/FreeCAD/releases
# Then install CfdOF: Tools → Addon Manager → CfdOF → Install
```

---

## 29. Plate Pair Spacing — Calculated Values and Surface Enhancement

### Convection Coefficients — Plain vs Enhanced Channels

With plain longitudinal channels, the hot side convection coefficient dominates:

| Channel | h_conv |
|---|---|
| Cold side (16 × 1.5 mm) | 113.7 W/m²K |
| Hot side (16 × 5.0 mm) | 29.3 W/m²K |
| **U — plain channels** | **23.3 W/m²K** |

With U = 23.3 W/m²K instead of 100, the area required is 4.3× larger — a stack height of ~1,655 mm per package. **Plain longitudinal channels are not usable.**

### Offset Strip Fin (OSF) Enhancement

| Geometry | U (W/m²K) | Stack height (per pkg) | Plates (+20%) | Status |
|---|---|---|---|---|
| Plain longitudinal | 23.3 | 1,655 mm — impractical | 988 | Not usable |
| OSF — conservative | **73** | **529 mm** | **158** | Workable |
| OSF — CFD-optimised (target) | **≥100** | **389 mm** | **116** | **Design target** |

OSF pressure drops remain well within limits (cold: 0.35 kPa, hot: 0.23 kPa vs limits of 19 kPa and 12 kPa respectively).

### Summary — Plate Pair Spacing Specification

| Parameter | Value |
|---|---|
| Cold channel clear height | **1.5 mm** |
| Hot channel clear height | **5.0 mm** |
| Plate foil thickness | **0.10 mm** |
| Cell pitch (one pair) | **6.70 mm** |
| Cold hydraulic diameter | **2.74 mm** |
| Hot hydraulic diameter | **7.62 mm** |
| Surface enhancement required | **Offset strip fin (OSF)** |
| OSF strip length | **6 mm** |
| U achieved (OSF, conservative) | **73 W/m²K** |
| U target with CFD optimisation | **≥ 100 W/m²K** |
| Stack height at U = 73 W/m²K | **529 mm** |
| Stack height at U = 100 W/m²K | **389 mm** — original Section 21 value |

---

## 30. Donor Vehicle Selection and ABS System

### Overview

The turbine car is built on a donor vehicle chassis. The donor's original ABS system is retained as standard equipment — complete, functional, and fully independent of the turbine engine control system. No modification to the ABS hardware is required; it operates exactly as it did from the factory.

The Continental/ATE MK60 ABS system, fitted as standard to the preferred BMW donor vehicles, operates without requiring external CAN bus communication from an engine ECU. This property — a deliberate design choice by Continental/ATE to allow the unit to be supplied to multiple vehicle manufacturers without bespoke software integration — makes it inherently compatible with any powerplant installation.

### Preferred Donor Vehicles

| Donor vehicle | Production | Cd | Frontal area | ABS system | Layout | Notes |
|---|---|---|---|---|---|---|
| **BMW E90 3-Series sedan** | 2005–2011 | **0.29** | **2.11 m²** | Continental/ATE MK60E1 or MK60E5 — standard | FR | **Preferred primary donor** — best compromise of size, weight, and ABS independence |
| BMW E46 3-Series sedan | 1998–2006 | 0.30 | 2.06 m² | Continental/ATE MK60 — standard from 2003 MY | FR | Wide availability; pre-2003 units use MK20 — verify before purchase |
| BMW E60 5-Series sedan | 2003–2010 | 0.27–0.28 | 2.26 m² | Continental/ATE MK60E1 or MK60E5 — standard | FR | Largest engine bay; heavier but more installation space |
| Mercedes-Benz W211 E-Class sedan | 2002–2009 | 0.28 | 2.10 m² | Bosch ABS — standard | FR | European taxi reference vehicle. Bosch ABS unit, not MK60 |
| Volkswagen Passat B6 sedan | 2005–2010 | 0.29 | 2.20 m² | Continental/ATE MK60 — standard on sport variants | FF or 4WD | Front-wheel-drive layout requires significant drivetrain modification |

### ABS System — Continental/ATE MK60

The Continental/ATE MK60 fitted to the BMW donor vehicles is a 4-channel ABS unit operating as a fully self-contained system requiring only wheel speed sensor inputs, brake pedal switch signal, power supply, and chassis ground.

| Parameter | MK60 / MK60E1 / MK60E5 |
|---|---|
| Manufacturer | Continental Automotive (formerly ATE / Teves) |
| Channels | 4-channel ABS — independent control of all four wheels |
| Standalone operation | **Yes — no external CAN bus or engine ECU required** |
| Donor vehicles | BMW E46 (MK60), BMW E90 (MK60E1/E5), BMW Z4, Mini R50/R53 |
| Wheel speed sensors | Hall-effect type — active sensors, 12V supply |
| Brake pedal switch | Grounded at rest, open when brake pressed (BMW convention) |
| Diagnostics | OBD-II port — readable with standard BMW diagnostics software |
| Reprogrammability | CSL firmware available for MK60 (E46 M3 813.3 / 817.3 variants) |

### Aerodynamic Reference — Donor Vehicle Cd Values

The BMW E90 sedan (Cd = 0.29, A = 2.11 m²) is taken as the primary aerodynamic reference. The W211 E-Class (Cd = 0.28, A = 2.10 m²) is the European taxi reference vehicle used to establish the design Cd target.

---

## 31. Cruise Power and Real-World Fuel Consumption

### Power Required at 80 km/h

Using the BMW E90 donor vehicle (Cd = 0.29, A = 2.11 m², mass 1,500 kg):

| Resistance component | Calculation | Force |
|---|---|---|
| Rolling resistance | Crr = 0.015, m = 1,500 kg, g = 9.81 m/s² | 221 N |
| Aerodynamic drag (80 km/h = 22.2 m/s) | ½ × 1.225 × 22.2² × 0.29 × 2.11 | 196 N |
| **Total resistance force** | — | **417 N** |
| **Power required at wheel** | 417 N × 22.2 m/s | **9.3 kW (12.5 HP)** |

### Comparison Across All Donor Vehicles at 80 km/h

| Donor vehicle | Cd | A (m²) | Aero drag | Total resistance | Wheel power needed |
|---|---|---|---|---|---|
| BMW E90 3-Series | 0.29 | 2.11 | 196 N | 417 N | 9.3 kW (12.5 HP) |
| BMW E46 3-Series | 0.30 | 2.06 | 199 N | 420 N | 9.3 kW (12.5 HP) |
| BMW E60 5-Series | 0.28 | 2.26 | 199 N | 420 N | 9.3 kW (12.5 HP) |
| Mercedes W211 E-Class | 0.28 | 2.10 | 185 N | 406 N | 9.0 kW (12.1 HP) |
| VW Passat B6 | 0.29 | 2.20 | 204 N | 425 N | 9.4 kW (12.6 HP) |

All donor vehicles require 9.0–9.4 kW (12–13 HP) at 80 km/h. Engine choice dominates fuel consumption far more than donor vehicle aerodynamics.

### RR300 Part-Load SFC Calculation

Gas turbine SFC increases significantly at part load:

$$SFC_{part} = SFC_{rated} \times \left(\frac{P_{rated}}{P_{actual}}\right)^{0.35}$$

$$SFC_{13HP} = 0.63 \times \left(\frac{210}{13}\right)^{0.35} = 0.63 \times 16.15^{0.35} = 0.63 \times 3.14 = \mathbf{1.98\ lb/SHP/hr}$$

| Parameter | Value |
|---|---|
| RR300 rated SFC (210 SHP cruise) | 0.63 lb/SHP/hr |
| Actual power at 80 km/h | ~13 HP (9.3 kW at wheel, η = 0.88) |
| Part-load SFC | **1.98 lb/SHP/hr** |
| Fuel flow at 13 HP (no recuperator) | 13 × 1.98 = 25.7 lb/hr = 13.2 L/hr |
| Fuel flow with recuperator (−30%) | 13.2 × 0.70 = **9.2 L/hr** |
| **Fuel consumption at 80 km/h** | 9.2 ÷ 80 × 100 = **11.5 L/100km** |

### Cruise Consumption Summary — All Engines

| Condition | Fuel flow | L/100km at 80 km/h |
|---|---|---|
| M250-C47B at full 450 SHP cruise (document figure) | 106 L/hr | 128 L/100km |
| RR300 at full 210 SHP cruise (document figure) | 48 L/hr | 58 L/100km |
| M250-C18 at full 220 SHP cruise (document figure) | 51 L/hr | 62 L/100km |
| **RR300 at actual 80 km/h road load (13 HP)** | **~9.2 L/hr** | **~11.5 L/100km** |
| **M250-C18 at actual 80 km/h road load (13 HP)** | **~9.5 L/hr** | **~11.9 L/100km** |
| Chrysler A-831 fleet average (1963–66) | — | 18.1 L/100km |
| Contemporary V8 equivalent (1963) | — | 15.7 L/100km |
| BMW E90 330i petrol (reference) | — | ~9.1 L/100km combined |

At genuine 80 km/h motorway cruise the RR300 or M250-C18 with recuperator achieves approximately **11.5–11.9 L/100km** — competitive with a 1960s V8 and substantially better than the Chrysler turbine car.

### Range Recalculated at 80 km/h Road Load

| Engine | Fuel flow at road load | 120 L cell duration | Range at 80 km/h |
|---|---|---|---|
| RR300 | ~9.2 L/hr | ~13 hours | **~1,040 km** |
| M250-C18 | ~9.5 L/hr | ~12.6 hours | **~1,008 km** |

These figures represent continuous cruising at a steady 80 km/h. A practical planning figure of **400–600 km on 120 litres** is realistic for mixed driving, compared with the 194–206 km figures at full cruise power in the range tables.

---

## 32. Reference Documents and Links

### Engine Documentation

- **Rolls-Royce M250-C18 Operation and Maintenance Manual:** https://miravim2.org/wp-content/uploads/2025/04/Allison-250-C18-Rolls-Royce-Operation-Maintenance-Manual.pdf
- **Bell 206B3 JetRanger Flight Manual:** https://www.mvheli.com/wp-content/uploads/bell-206b3-fm-1.pdf
- **FAA Type Certificate Data Sheet E3EA — M250 Engine Family:** https://rgl.faa.gov/Regulatory_and_Guidance_Library/rgMakeModel.nsf/0/E3EA
- **Robinson R66 Maintenance Manual (RR300 engine):** https://www.robinsonheli.com/r66-helicopter/

### FADEC and Electrical Interface

- **MIL-DTL-38999 Series III Connector Specification:** https://quicksearch.dla.mil/qsDocDetails.aspx?ident_number=34797
- **Albright SW180 Contactor:** https://www.albrightinternational.com/products/sw180/

### ABS System Reference

- **Continental/ATE MK60 standalone operation — E46 donor guide:** https://www.rusefi.com/forum/viewtopic.php?t=2454
- **MK60 / MK60E1 / MK60E5 swap reference:** https://www.lotustalk.com/threads/continental-bmw-mk60-mk60e1-mk60e5-abs-swap-thread.551646/

### Fuel Cell and Ancillary Systems

- **ATL Saver Cell Series:** https://www.atlinc.com/saver-cell-series.html
- **Hella UP30 Electric Vacuum Pump:** https://www.hella.com/microsite-electronics/en/UP30-32-vacuum-pump-117.html

### Heat Exchanger and CFD

- **OpenFOAM:** https://www.openfoam.com and https://www.openfoam.org
- **CfdOF FreeCAD Addon:** https://github.com/jaheyns/CfdOF
- **OpenFOAM CHT Tutorial:** https://wiki.openfoam.com/Conjugate_heat_transfer_by_Bruno_Santos
- **preCICE Heat Exchanger Tutorial:** https://precice.org/tutorials-heat-exchanger
- **Ansaldo AE-T100 (T100 recuperator source):** https://www.ansaldoenergia.com
- **Heatric PCHE:** https://www.heatric.com

### Regulatory and Historical

- **EU Euro 6 Emissions Regulation:** https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32007R0715
- **Chrysler Turbine Car Programme:** https://www.allpar.com/cars/turbine.html

---

## 33. Glossary

**AGM (Absorbed Glass Mat)** — A type of lead-acid battery capable of delivering the very high peak currents required for turbine starter motors. Used as two 12V/600A units in series to provide 24V startup supply.

**ATE MK60** — Continental/ATE four-channel ABS control unit fitted as standard to BMW E46, E90, and E60 donor vehicles. Operates fully standalone without external CAN bus communication, making it inherently compatible with non-OEM powerplant installations.

**B100** — Pure biodiesel — 100% fatty acid methyl ester (FAME) derived from vegetable oil or animal fat. Selected as the primary fuel for near-zero particulate emissions and complete renewable sourcing.

**CHT (Conjugate Heat Transfer)** — A simulation approach that simultaneously solves heat conduction through solid regions and convective heat transfer in fluid regions. Required for accurate recuperator simulation.

**chtMultiRegionFoam** — The OpenFOAM solver for conjugate heat transfer problems with multiple regions. The correct solver for recuperator simulation.

**Creep** — The slow permanent deformation of a material under sustained stress at elevated temperature. The primary life-limiting failure mechanism for turbine blades. Every 15°C reduction in TGT approximately doubles creep life.

**DLN (Dry Low NOx)** — A combustor design approach that premixes fuel and air before ignition, burning at a leaner, cooler mixture. Modern M250 family combustors achieve 15–40 ppm NOx versus 500+ ppm for the 1963 Chrysler A-831.

**EHPS (Electric Hydraulic Power Steering)** — A self-contained power steering pump driven by an electric motor. Required because the M250-C18 has no accessory belt drive to power a conventional hydraulic pump.

**Effectiveness (ε)** — A dimensionless measure of recuperator performance. The ratio of actual heat transfer to the maximum possible. Target: ε = 0.90 (90%).

**FADEC (Full Authority Digital Engine Control)** — A computer system that manages all aspects of engine fuel metering, starting, governing, and protection. Standard on the M250-C47B and RR300. The M250-C18 uses a hydromechanical FCU instead.

**FCU (Fuel Control Unit)** — The hydromechanical device on the M250-C18 that meters fuel flow. The Bendix/Honeywell DP-L2 FCU has three lever positions: OFF, IDLE, and RUN/FLY.

**FKM (Fluoroelastomer / Viton)** — An elastomeric seal material with excellent resistance to petroleum fuels, biodiesel, alcohols, and high temperatures. Specified throughout the fuel wetted circuit.

**FOD (Foreign Object Damage)** — Damage to compressor blades caused by ingestion of solid objects. Prevented in this design by the recuperator cold side channels acting as a natural filter.

**Hot Start** — A turbine start failure where TGT exceeds the start limit before N1 reaches self-sustaining speed. The most serious start failure mode. FADEC prevents hot starts automatically.

**Hung Start** — A turbine start failure where the engine lights off but fails to accelerate past a low N1. Most common cause in automotive installation: low battery voltage producing a slow starter motor.

**LMTD (Log Mean Temperature Difference)** — The effective driving temperature difference across a heat exchanger. For the M250-C18 recuperator at ε = 0.90, LMTD = 22°C.

**NOx (Nitrogen Oxides)** — The primary regulatory challenge for gas turbine automotive applications. The reason the Chrysler turbine car programme was discontinued in 1979. Modern DLN combustors achieve 15–40 ppm versus 500+ ppm for 1960s designs.

**NTU (Number of Transfer Units)** — A dimensionless heat exchanger design parameter. For ε = 0.90 in counterflow, NTU ≈ 9.0.

**OSF (Offset Strip Fin)** — A heat exchanger surface enhancement where the fin is divided into short strips, each offset laterally. Interrupts the thermal boundary layer and substantially increases the convection coefficient. Required to achieve U ≥ 73 W/m²K.

**Part-Load SFC** — Specific fuel consumption at power settings below rated cruise. Gas turbines are least efficient at deep part load. At 13 HP versus 210 HP rated, the RR300 SFC increases from 0.63 to approximately 1.98 lb/SHP/hr.

**Primary Surface Recuperator (PSR)** — A heat exchanger where the primary heat transfer surface is the thin metal plate itself, using 0.10 mm SS347 stainless steel foil, vacuum brazed or laser welded.

**Recuperator** — A static, counterflow, gas-to-gas heat exchanger that transfers heat from the turbine exhaust to the compressed air before it enters the combustor. Has no moving parts. Reduces fuel consumption by approximately 30%.

**SFC (Specific Fuel Consumption)** — The fuel flow per unit of shaft power output. For the M250-C18, SFC = 0.64 lb/SHP/hr at rated cruise. The recuperator reduces effective SFC by approximately 30%.

**SS347 (Stainless Steel 347)** — An austenitic stainless steel alloy with excellent high-temperature strength and oxidation resistance to approximately 675°C sustained. The standard material for gas turbine primary surface recuperators at 0.10 mm foil thickness.

**TBO (Time Between Overhaul)** — The manufacturer-specified overhaul interval. M250-C18 Series II: 3,500 hours. M250-C47B and RR300: 2,000 hours.

**TGT (Turbine Gas Temperature)** — The temperature of the gas between the gas producer turbine and the power turbine. The primary indicator of engine health and the most important limit to monitor during starting and operation.

**U (Overall Heat Transfer Coefficient)** — Combines the convection resistances on both fluid sides and the conduction resistance of the separating wall. Design assumption: 100 W/m²K. Plain longitudinal channels achieve 23.3 W/m²K; OSF geometry achieves 73–100 W/m²K.

**Vacuum Brazing** — A joining process where heat exchanger plates are assembled with brazing alloy, placed in a vacuum furnace, and heated until the alloy flows and bonds the plates. The standard joining method for SS347 primary surface recuperators.

**Zeldovich Mechanism** — The dominant chemical pathway for thermal NOx formation. Atmospheric nitrogen dissociates at temperatures above approximately 1,500°C. NOx production increases exponentially with flame temperature — the reason DLN combustors, biodiesel, and water injection all reduce NOx.

---

*End of specification document.*
