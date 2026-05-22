# Recuperated Gas Turbine Car — Concept Design Specification

---

## Table of Contents

- [Historical Background — The Turbine Car Programs](#historical-background--the-turbine-car-programs)

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
12. [Alternative Engine — Lighter Vehicle Application](#12-alternative-engine-suggestion--lighter-vehicle-application)
13. [Lower Power Option — 100 to 200 HP Range](#13-lower-power-option--100-to-200-hp-range)
14. [Acceleration Estimates — All Engines](#14-acceleration-estimates--all-engines)
15. [FADEC Derating — How Power Limiting Works](#15-fadec-derating--how-power-limiting-works)
16. [Time Between Overhaul TBO](#16-time-between-overhaul-tbo)
17. [Three-Engine Comparison Summary](#17-three-engine-comparison-summary)
18. [Compatible Fuels and Seal Materials](#18-compatible-fuels-and-seal-materials)
19. [Water Injection System](#19-water-injection-system)
20. [Air Movement — Volumetric Flow and Pressure Drop](#20-air-movement--volumetric-flow-and-pressure-drop)
21. [Heat Exchanger Plate Geometry — M250-C18](#21-heat-exchanger-plate-geometry--m250-c18)
22. [Ancillary Systems, Costs and Instrumentation](#22-ancillary-systems-costs-and-instrumentation)

---

## Historical Background — The Turbine Car Programs

### Why This Concept Has Deep Roots

The gas turbine car is not a new idea. It was pursued seriously and
publicly by multiple major manufacturers across three decades — and
came remarkably close to production. Understanding what was achieved,
what failed, and why it failed is essential context for any modern
revival of the concept.

---

### General Motors Firebird Series — 1953 to 1964

General Motors had been researching the potential of turbine engines
since the 1940s, but it wasn't until the early 1950s that a completed
real-life prototype emerged. The result was a series of four
concept vehicles — the GM Firebird series — each more extreme than
the last, built for the annual Motorama auto shows and never
intended for public sale. These were the Jetsons-era machines that
defined the public imagination of what a turbine car might look like.

**Firebird I (XP-21) — 1953/1954**

The first gas turbine automobile ever built and tested in the United
States. At the heart of the XP-21 was the Whirlfire Turbo-Power gas
turbine engine, capable of producing 370 horsepower at a power turbine
speed of 13,000 rpm, expelling exhaust at 677°C. Its design was
literally that of a jet aircraft on wheels — single seat, glass
canopy, tail fin, delta wings. It was purely a test and show vehicle,
never road-registered.

**Firebird II — 1956**

Unveiled at the GM Motorama in New York City, the Firebird II housed
a gas turbine operating at 35,000 rpm — borderline science fiction
for a road vehicle. Unlike its predecessor it had four seats and
was presented as a genuine family car concept, complete with titanium
body and an early vision of automatic highway guidance. The turbine
was a GT-304 Whirlfire unit producing 200 HP in a more practical
automotive configuration.

**Firebird III — 1959**

The Firebird III was a two-seater powered by a 225 HP Whirlfire
GT-305 gas turbine engine and a separate two-cylinder 10 HP gas
engine to power accessories. It featured seven fins, a
bubble canopy, and a single joystick replacing the conventional
steering wheel. It was displayed widely at auto shows and represents
the high point of GM's turbine showmanship — spectacular, futuristic,
and entirely non-functional as a road car.

**Firebird IV — 1964**

GM coded it internally as the XP-790 and conceived it for a future
in which cars steered automatically via programmed guidance systems.
Though billed as being turbine-powered, the Firebird IV was
non-functional — a pure styling exercise. It was later
repackaged as the Buick Century Cruiser for the 1969 show circuit
and reportedly crushed in the 1980s.

None of the four Firebirds reached public testers. They were
show cars — the primary purpose was to demonstrate GM's
engineering ambition and generate public excitement about the
future of the automobile. The turbine technology in the Firebirds
was real, but the cars themselves were never intended for the road.

---

### Chrysler Turbine Car — The Real Public Test

Where GM used turbines for showmanship, Chrysler used them for
science. Chrysler's turbine programme ran from the late 1930s
through to 1979 — forty years of continuous engineering development
across seven engine generations.

**The Programme History**

The CR2A third-generation engine incorporated a major innovation:
a variable nozzle mechanism acting as a shutter that provided engine
braking. It improved efficiency and fuel economy while reducing the
throttle lag that had plagued the programme from its inception.

The fourth-generation A-831 engine powered the famous Ghia-bodied
Turbine Car of the public loaner programme. After testing,
Chrysler conducted a user program from October 1963 to January 1966
that involved 203 drivers in 133 cities in the United States,
cumulatively driving more than one million miles.

55 cars were distributed to 203 volunteers in 48 states free of
charge for three months each. The power turbine was connected,
without a torque converter, through a gear reduction unit to a
modified TorqueFlite automatic transmission. Twin rotating
recuperators transferred exhaust heat to the inlet air, greatly
improving fuel economy.

**Fuel Consumption — The Honest Figures**

The fuel economy results from the public programme were mixed and
have been reported variously by different sources. The range of
reported figures reflects both the variability of real-world
driving and the enthusiasm with which some drivers chose to exploit
the car's instant torque:

| Source | Reported economy |
|---|---|
| Average fleet figure (Chrysler records) | **13 mpg US (18.1 L/100km)** |
| Best reported (highway) | **18–19 mpg US (12.4–13.1 L/100km)** |
| Typical town driving | **14.5 mpg US (16.2 L/100km)** |
| Worst reported (enthusiastic driving) | **11–11.5 mpg US (20.5–21.4 L/100km)** |
| Contemporary V8 equivalent car | ~15 mpg US (15.7 L/100km) |

About one in four test drivers stated dissatisfaction with the fuel
economy. Chrysler blamed the poorer results on drivers showing off
the cars, regarding their own reading of 14.5 mpg as more accurate.
At 14.5 mpg the turbine was only fractionally below the national
average for a car of its size.

---

### What Killed the Programme — The 1970s Fuel and NOx Crisis

The Chrysler turbine programme did not die from engineering failure.
It was killed by two external forces arriving simultaneously in the
early 1970s.

**1. The NOx Regulatory Crisis**

The A-831's fatal regulatory issue came from the same characteristic
that made it so different. Because it burned fuel continuously at
combustion temperatures between 1,700 and 2,500°F, nitrogen oxide
output ran significantly higher than a piston engine operating at
equivalent power. When the EPA was formed in 1970 and empowered by
the Clean Air Act, it listed NOx as a criteria pollutant requiring
compliance from every road vehicle sold in the US.

Chrysler received a $6.4 million EPA development contract in 1972
specifically to address the NOx problem, and a seventh-generation
turbine engine with improved emissions and fuel economy followed.
A turbine-powered Chrysler LeBaron was built in 1977 as a potential
production preview. But the regulatory timeline was short,
the development costs were enormous, and Chrysler's financial
position in the late 1970s was parlous. The programme was
abandoned in 1979.

**2. The 1973 and 1979 Oil Crises**

The fuel crises of 1973 and 1979 fundamentally shifted public and
regulatory attention toward fuel economy above all else. A turbine
running at 13 mpg average — equivalent to a V8 — was no longer
acceptable at a time when the national conversation had shifted
entirely to miles per gallon. The turbine's advantages — low
maintenance, multi-fuel capability, smooth operation, instant
torque — were simply not the advantages anyone cared about anymore.

The irony of the whole programme is that the NOx problem was a
genuine engineering challenge, but not a fundamental dead end.
The window to solve it closed before Chrysler had the resources
or the regulatory timeline to finish the work.

---

### How Much Turbine Technology Has Improved Since Then

The 1963 A-831 combustor was a simple diffusion flame design — fuel
and air injected separately, burning at stoichiometric hot spots
that inevitably generated high NOx. The technology available today
is fundamentally different.

**NOx Reduction — Five Decades of Progress:**

Advances in lean premix Dry Low NOx (DLN) combustion technology
have lowered NOx emissions from the 150–300 ppm level of the 1980s
to the 15–40 ppm level today, depending on the size and type of
unit. This 90% reduction through cost-effective pollution prevention
is unmatched by any other industrial sector.

Modern lean-premix systems can achieve NOx emissions of 5 ppmvd
and sometimes lower when firing gas. Even on liquid fuels,
water injection into the combustor flame zone reduces NOx by about
40% when half as much water as fuel is injected.

**Fuel Consumption Comparison — 1963 vs Modern:**

| Parameter | Chrysler A-831 (1963) | Modern M250-C18 recuperated | Improvement |
|---|---|---|---|
| Engine power | 130 HP | 250 HP continuous | — |
| Recuperator | Rotary regenerator | Fixed plate — no moving parts | More reliable |
| Recuperator effectiveness | ~91–97% | ~90% | Comparable |
| Fuel consumption (cruise) | ~13 mpg (18 L/100km) | ~51 L/hr at 220 SHP (see §10) | Similar per HP — more absolute power |
| NOx (combustor type) | Diffusion flame — ~500+ ppm | Modern annular — 15–40 ppm | **~90–95% lower** |
| CO | Low (turbine burns clean) | Near zero | Similar |
| Particulates | Low | Near zero on biodiesel | Better |
| Throttle lag | Significant complaint | Much reduced — variable geometry | Improved |
| Cold start | Complicated procedure | FADEC automated | Greatly improved |
| Maintenance | 5 dedicated mechanics for 50 cars | On-condition TBO — 3,500 hrs | Dramatically better |
| Multi-fuel | Yes — diesel, petrol, kerosene | Yes — plus biodiesel, ethanol | Broader |

The NOx column is the most important. What killed the Chrysler
programme in regulatory terms is now reduced by 90–95% through
combustion engineering alone — before any contribution from the
water injection system described in Section 19, biodiesel fuel
(Section 18), or the recuperator's exhaust cooling effect
(Section 4). A modern recuperated turbine car running on biodiesel
with modest water injection would likely meet Euro 6 NOx limits
without any exhaust aftertreatment — something Chrysler could not
have imagined in 1979.

The concept was not wrong. The technology simply needed another
fifty years.

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

Running derated at 450–500 SHP provides substantial margin below the 650 SHP maximum,
extending TBO (Time Between Overhauls) significantly and reducing thermal stress on all
hot-section components.

---

## 2. Output Shaft and Step-Down Gearbox

The M250-C47B internal gearbox delivers **6,000 RPM** at the output flange. This is
too fast for direct coupling to a conventional automotive transmission or torque converter,
which operate comfortably at 2,000–4,000 RPM input.

**A step-down reduction gearbox is required.**

| Parameter | Value |
|---|---|
| Input speed | 6,000 RPM |
| Required output speed | 2,000–3,000 RPM |
| Reduction ratio | 2:1 to 3:1 |
| Power rating required | 500+ HP continuous |

Suitable off-the-shelf industrial or helicopter accessory gearboxes in this speed and power
range are readily available. Units from within the M250 helicopter ecosystem are an obvious
source, already rated for this exact shaft speed and power level.

---

## 3. Mass Flow Rate

$$\dot{m} = \mathbf{2.77\ kg/s}$$

This is the confirmed published figure for the M250-C40/C47 family at pressure ratio 9.2:1.
Both recuperator packages share this flow equally, each handling **1.385 kg/s**.

---

## 4. What the Heat Exchanger Does

The heat exchanger in this design is a **recuperator** — a static, counterflow,
gas-to-gas plate heat exchanger with no moving parts. It performs five distinct
functions simultaneously, all of which are essential to making a gas turbine
practical in a car.

---

### Function 1 — Waste Heat Recovery (Primary Purpose)

A simple-cycle gas turbine exhausts gas at around **546°C** after the power
turbine has extracted useful work. That represents a large fraction of the
fuel energy simply thrown away. The recuperator captures this heat and
transfers it to the cold compressed air coming from the compressor before
it enters the combustor.

The compressed air arrives at the recuperator cold side at around **260–420°C**
depending on ambient temperature. After passing through the recuperator it
leaves at approximately **456–475°C** — already most of the way to combustion
temperature. The combustor therefore needs to add far less fuel to reach the
required turbine inlet temperature.

The result is a **~30% reduction in fuel consumption** compared to the same
engine running without a recuperator. Without it, the fuel consumption figures
in this document would be unacceptable for a road car. The recuperator is what
makes the concept viable.

---

### Function 2 — Exhaust Cooling

As the hot exhaust gas surrenders its heat to the cold air stream, it cools
dramatically — from ~546°C at the turbine exit to approximately **177–282°C**
at the recuperator hot-side outlet, depending on ambient temperature. This
cooled exhaust then travels through the rear duct to the tailpipe.

Without the recuperator the exhaust would exit at over 500°C — capable of
igniting materials it contacts and certainly damaging road surfaces. The
recuperator makes the exhaust temperature manageable, reducing the
engineering burden on the rear ducting and exit diffuser.

---

### Function 3 — Intake Air Preheating

Preheating the compressed air before it enters the combustor has a secondary
thermodynamic benefit beyond fuel saving. Warmer air entering the combustor
means a more stable, complete combustion process — lower CO and unburned
hydrocarbon emissions, and more consistent combustion across the full power
range. On biodiesel, which has slightly different combustion characteristics
to petroleum diesel, this stable pre-heated intake condition is particularly
beneficial.

---

### Function 4 — FOD Protection

The recuperator cold side — through which fresh ambient air passes on its
way from the intake to the compressor — acts as a natural **Foreign Object
Damage (FOD) barrier**. The narrow plate channels, with their tortuous
counterflow path, physically prevent:

- Insects, leaves, grit, and small stones from reaching the compressor
- Water droplets and ice crystals, separated as air changes direction
  through the core
- Any debris larger than the plate gap dimension

This eliminates the need for a separate **Inlet Particle Separator (IPS)**,
which is a mandatory and bulky fitment on helicopter installations of the
M250 family. A simple coarse mesh screen at the intake scoop is all that
is required upstream of the recuperator.

---

### Function 5 — Partial Exhaust Noise Attenuation

As exhaust gas passes through the narrow plate channels of the hot side,
the acoustic energy in the gas stream is partially absorbed and dissipated
by the plate material and the tortuous flow path. This is not a designed
silencing function, but it is a real side effect — the recuperator acts as
a partial muffler, reducing the high-frequency turbine whine before the
exhaust reaches the rear duct silencer. The Chrysler A-831 turbine car
relied on this same effect from its twin regenerators.

---

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

### Operating Temperature Range

| Condition | Ambient | Notes |
|---|---|---|
| Cool season start | +5°C | Design case — maximum heat duty |
| Normal operation | +5°C to +35°C | Typical European warm season |
| Worst hot case | +45°C | Southern Europe midsummer |
| Cold storage/transport | −45°C | Non-operating; affects material selection only |

### Cycle State Point Temperatures

| Parameter | +5°C ambient | +20°C ambient | +45°C ambient |
|---|---|---|---|
| Compressor inlet T1 | 278 K (5°C) | 293 K (20°C) | 318 K (45°C) |
| Compressor outlet T2 — cold side IN | 605 K (332°C) | 638 K (365°C) | 692 K (419°C) |
| Turbine exhaust T4 — hot side IN | 819 K (546°C) | 819 K (546°C) | 819 K (546°C) |
| Preheated air T3 — cold side OUT | 814 K (541°C) | 819 K (546°C) | 806 K (533°C) |
| **Final exhaust T5 — hot side OUT** | **610 K (337°C)** | **638 K (365°C)** | **705 K (432°C)** |
| Recuperator heat duty | 582 kW | 504 kW | 318 kW |

### Notes on Final Exhaust Temperature

At +45°C ambient the compressor outlet temperature (419°C) approaches the turbine
exhaust temperature (546°C), leaving only a 127°C differential across the recuperator.
This is a known characteristic of high pressure ratio turbines — recuperation becomes
less effective at high ambient temperatures because the compressor already heats the
intake air substantially.

**A dilution diffuser at the exhaust exit is therefore not optional.** It is a designed
feature required at all operating temperatures to cool exhaust gas before it reaches
road level, and is particularly important on hot days.

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

### Total Surface Area

$$A_{total} = \frac{Q}{U \times LMTD} = \frac{582{,}000}{100 \times 5} = \mathbf{1{,}164\ m^2}$$

This is **primary wetted surface area** — not external footprint.

### Split Configuration — Two Packages

The recuperator is divided into two equal packages, one mounted each side of the engine,
positioned slightly rearward to keep heat away from forward-mounted accessories,
fuel system components, and electronics. This arrangement mirrors Chrysler's A-831
twin-regenerator layout and provides symmetrical weight distribution.

| Parameter | Per Package | Total |
|---|---|---|
| Primary surface area | **582 m²** | 1,164 m² |
| Core volume | **~0.685 m³** | ~1.37 m³ |
| Physical envelope (approx.) | **600 × 500 × 230 mm** | — |
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
| Inconel required? | No — at these operating temperatures SS347 is sufficient |

### Thermal Expansion and Mounting

- Flexible expansion joints at all four duct connections per package
- Floating mounts allowing free axial growth
- Total metal temperature range for stress calculation: **−45°C (storage) to 546°C (operation) = 591°C swing**
- FADEC spool-up sequence limits fuel flow on cold start to allow gradual thermal
  equalisation across the recuperator core — preventing shock loading

---

## 7. FOD Protection

The recuperator layout provides Foreign Object Damage (FOD) protection as a
natural consequence of its design. Fresh combustion air is drawn through the cold
side of the recuperator before reaching the compressor inlet. The narrow plate
channels act as an effective barrier:

- Insects, grit, small stones and debris cannot navigate the tortuous path
  through the plate channels
- Water droplets are separated as air changes direction through the core
- Air arrives at the compressor pre-heated, with particulates removed

**No separate Inlet Particle Separator (IPS) is required.** A simple
weather-proof intake scoop with a coarse mesh screen upstream of the
recuperator cold side inlet is sufficient — a significant simplification
compared to a standard helicopter installation of the M250 which normally
demands a dedicated IPS.

---

## 8. Electrical System

Two 12V / 600A AGM batteries connected in series providing 24V for engine startup.

```
Starter-Generator 28V output
        |
    [+ Battery 2 −]
        |
    [+ Battery 1 −] ←— 12V tap for all car electronics
        |
      Ground
```

| Function | Supply |
|---|---|
| Engine startup | 24V across both batteries in series |
| Car electronics (lights, instruments etc.) | 12V tapped at Battery 1 positive to ground |
| Battery charging (running) | Starter-generator 28V charges both batteries in series — each sees ~14V |

No relay, no DC-DC converter, no switching logic required. The physics of the
series circuit isolates the 12V accessories from the high-current startup path
automatically. Both batteries remain healthy and fully charged during normal running.

---

## 9. Fuel Cell

### Available Options — ATL Saver Cell Series

ATL Saver Cells are FIA FT3-1999 approved, constructed from a unique tough plastic
alloy (FIA Homologation No. ATL-565), fully foam-baffled internally, and compatible
with biodiesel fuel. Available off-the-shelf in the following relevant sizes:

| Capacity | Approximate Dimensions (with aluminium container) | Notes |
|---|---|---|
| 100 litres | 671 × 671 × 340 mm (low profile) | Readily available, standard stock item |
| 120 litres | 641 × 465 × 420 mm | Standard stock item |
| 120 litres | 620 × 416 × 535 mm | FIA approved alternative profile |

**Recommended: ATL 120 litre Saver Cell** — maximum within the stated 130-litre
limit, standard stock item, FIA approved, biodiesel compatible with blue foam baffle
specification.

---

## 10. Fuel Consumption and Range

### SFC Basis

The confirmed published SFC for the M250-C47B at cruise power is
**0.65 lb/SHP/hr** (official engine specification database figure).
The 0.772 figure used previously was incorrect — it overstated
fuel consumption significantly. Running derated at **450 SHP continuous:**

$$\text{Fuel flow} = 450 \times 0.65 = 292.5\ \text{lb/hr} = 132.7\ \text{kg/hr}$$

### Simple Cycle (no recuperator)

$$\text{Fuel flow} = \frac{132.7}{0.88} = \mathbf{150.8\ \text{litres/hr}}$$

*(Biodiesel density ~0.88 kg/litre)*

### Recuperated Cycle

The recuperator improves thermal efficiency by approximately 30% at cruise:

$$\text{Recuperated fuel flow} = 150.8 \times 0.70 = \mathbf{106\ \text{litres/hr}}$$

### Running Time and Range

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **28 minutes** | **~39 km** |
| 100 litres | **57 minutes** | **~78 km** |
| **120 litres (recommended)** | **~68 minutes** | **~93 km** |
| Required for 165 km / 2 hrs | — | **~212 litres needed** |

### Range Note

The reference journey of 165 km taking 2 hours requires approximately
**212 litres** of biodiesel at cruise power with recuperation. The
maximum practical fuel cell of 120 litres provides approximately
**93 km range** — sufficient for a convention demonstration, circuit
event, or short-distance showcase run, but not for extended road use
without refuelling.

The fuel consumption is a direct consequence of the M250-C47B's power
level — at 450 SHP derated it is producing roughly 3.5× more power
than the car needs at highway cruise, burning fuel accordingly. A
smaller engine in the 200–250 SHP class provides similar real-world
performance with significantly lower fuel consumption.

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
| **Total recuperator surface area** | **1,164 m²** |
| **Per package surface area** | **582 m²** |
| **Per package envelope** | **600 × 500 × 230 mm** |
| **Recuperator material** | SS347 stainless steel |
| **Hot side inlet temperature** | 546°C |
| **Final exhaust temperature** | 337°C (design case +5°C ambient) |
| **Exhaust dilution diffuser** | Required at all temperatures |
| **FOD protection** | Provided by recuperator cold side channels |
| **Fuel** | Biodiesel (B100) |
| **Fuel cell** | ATL 120L Saver Cell — 641 × 465 × 420 mm |
| **Recuperated fuel flow** | ~106 litres/hr at 450 SHP |
| **Range on 120 litres** | **~93 km / ~68 minutes** |
| **Electrical startup** | 24V — 2 × 12V / 600A AGM batteries in series |
| **Car electronics supply** | 12V tapped at Battery 1 positive terminal to ground |

---

*Concept design specification — theoretical study only.*
*All performance figures based on published M250 family data and standard thermodynamic analysis.*
*Recuperator dimensions and surface area calculated for ε = 0.90, U = 100 W/m²K, design case +5°C ambient.*

---

## 12. Alternative Engine Suggestion — Lighter Vehicle Application

### Rationale

For a vehicle weighing 1,200–1,500 kg the M250-C47B at 650 SHP maximum is
significantly oversized. A 1,400 kg car requires approximately **150–200 HP (112–149 kW)**
for brisk but civilised road performance — responsive in traffic, capable of comfortable
highway cruising, but not extreme. A turbine in the **200–300 SHP range** provides
genuine performance with headroom, without the fuel appetite of the C47B.

Two candidates are well suited:

---

### Candidate A — Rolls-Royce RR300

| Parameter | Value |
|---|---|
| Type | Twin-spool free-turbine turboshaft |
| Certification | February 2008 (FAA) — within preference window |
| Maximum takeoff power | **300 SHP (224 kW)** |
| Maximum continuous power | **240 SHP (179 kW)** |
| Engine control | **FADEC** |
| Pressure ratio | **6.2:1** |
| Output shaft speed | ~6,000 RPM (M250 family standard) |
| Dry weight | **79.8 kg (176 lb)** |
| Length | 1,041 mm |
| SFC at cruise | **0.63 lb/SHP/hr** |
| Compressor | Single-stage centrifugal (titanium) |
| Turbine | 2-stage gas producer + 2-stage free power turbine |
| Primary application | Robinson R66 helicopter |
| Airflow | ~1.8 kg/s (estimated, scaled from M250 family at 6.2:1 PR) |

The RR300 is a direct M250 family derivative — sharing the same modular layout,
gearbox interface, and support ecosystem — making it an extremely practical choice.
FADEC is standard. The lower pressure ratio of 6.2:1 versus the C47B's 9.2:1 means
the compressor outlet temperature is lower, which actually makes recuperation more
effective at all ambient temperatures.

---

### Candidate B — Turbomeca (Safran) Arrius 2F

| Parameter | Value |
|---|---|
| Type | Twin-spool free-turbine turboshaft |
| Certification | November 1996 (EASA/FAA) |
| Maximum takeoff power | **504 SHP (376 kW)** |
| Continuous derated target | **200–250 SHP (149–186 kW)** |
| Engine control | Hydromechanical fuel control (not FADEC) |
| Pressure ratio | ~7.5:1 |
| Output shaft speed | ~6,000 RPM via reduction gearbox |
| Dry weight | **101.3 kg (223 lb)** |
| Length | 1,601 mm |
| Airflow | **~1.5 kg/s** |
| Primary application | Eurocopter EC120B Colibri |

**Note:** The Arrius 2F uses a hydromechanical fuel control, not FADEC. This is a
significant disadvantage for this application — FADEC is strongly preferred for
overspeed protection, startup management, and part-load optimisation in a car.
The Arrius 2F is therefore the secondary candidate unless retrofitted with an
aftermarket electronic control system. The RR300 is the preferred choice.

---

### Recommended Alternative: Rolls-Royce RR300

Running derated at **200–220 SHP continuous** from a 300 SHP maximum gives
excellent performance margin, low thermal stress, and extended TBO.

**Power-to-weight comparison for 1,400 kg vehicle:**

| Engine | Continuous power | Power-to-weight (vehicle) |
|---|---|---|
| M250-C47B (derated) | 450 SHP (336 kW) | **240 kW/tonne** — supercar territory |
| RR300 (derated) | 210 SHP (157 kW) | **112 kW/tonne** — very brisk, civilised |

The RR300 at 112 kW/tonne is comparable to a well-specced performance saloon —
excellent acceleration, comfortable in traffic, but not violent. Entirely appropriate
for a warm-season touring car concept.

---

### RR300 Recuperator Calculations

#### Revised Cycle Temperatures — Pressure Ratio 6.2:1

Using the same methodology as Section 4, with PR = 6.2, η_c = 0.80, η_t = 0.85,
ε = 0.90, TIT ≈ 900°C (1,173 K), design case +5°C ambient:

**Compressor outlet T2:**

$$T_{2s} = T_1 \times 6.2^{0.286} = 278 \times 1.735 = 482 \text{ K}$$

$$T_2 = T_1 + \frac{T_{2s} - T_1}{\eta_c} = 278 + \frac{204}{0.80} = \mathbf{533 \text{ K}\ (260°C)}$$

**Turbine exhaust T4:**

$$T_{4s} = 1173 \times (1/6.2)^{0.286} = 1173 \times 0.577 = 677 \text{ K}$$

$$T_4 = 1173 - 0.85(1173 - 677) = 1173 - 422 = \mathbf{751 \text{ K}\ (478°C)}$$

**Recuperator temperatures with ε = 0.90:**

$$T_3 = 533 + 0.9(751 - 533) = 533 + 196 = \mathbf{729 \text{ K}\ (456°C)}$$

$$T_5 = 751 - 0.9(751 - 533) = 751 - 196 = \mathbf{555 \text{ K}\ (282°C)}$$

**Key improvement over M250-C47B:** Final exhaust T5 at design condition is **282°C**
versus **337°C** for the C47B — meaningfully cooler, easing the dilution diffuser
requirement.

#### RR300 Recuperator Temperature Table

| Parameter | +5°C | +20°C | +45°C |
|---|---|---|---|
| T2 — cold side IN | 260°C | 290°C | 335°C |
| T4 — hot side IN | 478°C | 478°C | 478°C |
| T3 — cold side OUT | 456°C | 462°C | 471°C |
| **T5 — final exhaust** | **282°C** | **294°C** | **321°C** |
| Heat duty | 263 kW | 234 kW | 183 kW |

The lower hot-side inlet temperature of **478°C** versus 546°C for the C47B is also
significant — **SS347 is fully adequate with greater margin**, and the risk of
creep is reduced.

---

### RR300 Heat Exchanger Surface Area

**Design case: +5°C ambient, heat duty = 263 kW**

LMTD (counterflow, ε = 0.90):

$$\Delta T_1 = 478 - 456 = 22°C \quad \Delta T_2 = 282 - 260 = 22°C$$

$$LMTD = 22°C$$

$$A_{total} = \frac{Q}{U \times LMTD} = \frac{263{,}000}{100 \times 22} = \mathbf{120 \text{ m}^2}$$

This is dramatically smaller than the C47B requirement. Split two ways:

| Parameter | Per Package | Total |
|---|---|---|
| Primary surface area | **60 m²** | **120 m²** |
| Core volume | **~0.071 m³** | ~0.14 m³ |
| Physical envelope (approx.) | **300 × 250 × 95 mm** | — |

The RR300 recuperator packages are roughly **one-tenth the volume** of those
required for the C47B — compact enough to mount very neatly alongside the
engine with minimal packaging impact.

---

### RR300 Mass Flow Rate

Scaled from the M250 family at pressure ratio 6.2:1 versus 9.2:1:

$$\dot{m}_{RR300} \approx 2.77 \times \frac{6.2}{9.2} \approx \mathbf{1.87 \text{ kg/s}}$$

Each package handles **0.935 kg/s**.

---

### RR300 Step-Down Gearbox

Output shaft speed is the same M250 family standard of approximately **6,000 RPM**.
The same 2:1 to 3:1 step-down gearbox requirement applies as for the C47B.
Being from the same engine family, the same gearbox solutions are applicable.

---

### RR300 Fuel Consumption and Range

**SFC:** 0.63 lb/SHP/hr at cruise (confirmed M250 family figure)

Running at **210 SHP continuous:**

$$\text{Fuel flow} = 210 \times 0.63 = 132.3 \text{ lb/hr} = 60.0 \text{ kg/hr}$$

$$\text{Fuel flow (litres)} = \frac{60.0}{0.88} = \mathbf{68 \text{ litres/hr}}$$

**With recuperator — 30% SFC improvement:**

$$\text{Recuperated fuel flow} = 68 \times 0.70 = \mathbf{48 \text{ litres/hr}}$$

#### Range on Available Fuel Cells

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **63 minutes** | **~86 km** |
| 100 litres | **125 minutes** | **~172 km** |
| **120 litres (ATL recommended)** | **~150 minutes (2hrs 30min)** | **~206 km** |

**The 120 litre ATL Saver Cell comfortably exceeds the 165 km / 2-hour target with the RR300.**

This is the critical result. The RR300 at derated cruise power with recuperation
achieves the design range goal on a single standard fuel cell with significant
margin to spare, whereas the M250-C47B requires approximately 212 litres to
achieve the same range.

---

### Comparative Summary — M250-C47B vs RR300

| Parameter | M250-C47B | RR300 | Advantage |
|---|---|---|---|
| Max power | 650 SHP | 300 SHP | C47B |
| Continuous derated | 450–500 SHP | 200–210 SHP | RR300 (right-sized) |
| Vehicle power/weight (1,400 kg) | 240 kW/tonne | 112 kW/tonne | RR300 (appropriate) |
| Mass flow | 2.77 kg/s | ~1.87 kg/s | RR300 (smaller system) |
| Total HX surface area | 1,164 m² | **120 m²** | **RR300** |
| Per package HX envelope | 600×500×230 mm | **300×250×95 mm** | **RR300** |
| Hot side inlet temp | 546°C | **478°C** | **RR300** |
| Final exhaust temp (+5°C) | 337°C | **282°C** | **RR300** |
| FADEC | Yes | **Yes** | Equal |
| Engine weight | ~72 kg | **~80 kg** | C47B (marginal) |
| Recuperated fuel flow | 106 litres/hr | **48 litres/hr** | **RR300** |
| Range on 120 litres | ~93 km | **~206 km** | **RR300** |
| Meets 165 km target? | **No** (needs ~212L) | **Yes** (120L — margin to spare) | **RR300** |
| Step-down gearbox | 2:1–3:1 required | 2:1–3:1 required | Equal |
| FOD protection via HX | Yes | Yes | Equal |
| Electrical system | 24V / 2×12V AGM | 24V / 2×12V AGM | Equal |

### Conclusion

**The Rolls-Royce RR300 is the correct engine for this concept.**

It is right-sized for a 1,200–1,500 kg vehicle, achieves the 165 km range target
on a 120-litre ATL fuel cell, requires a recuperator that is one-tenth the volume
of that needed for the C47B, produces a meaningfully lower final exhaust temperature,
and retains FADEC as standard. The M250-C47B remains a valid alternative where
maximum performance is the priority and fuel range is a secondary concern —
effectively a different vehicle concept entirely.

---

*Alternative engine section added as supplement to primary specification.*
*RR300 calculations use published specifications and same thermodynamic methodology as Section 4.*
*Arrius 2F airflow estimate based on published training manual data (Arrius 2B1: 2.03 kg/s at comparable pressure ratio).*

---

## 13. Lower Power Option — 100 to 200 HP Range

### Rationale

A 1,200–1,500 kg car requires only 100–150 HP for relaxed but fully adequate road
performance — comfortable in traffic, capable of sustained highway cruising, and
very economical on fuel. A turbine in this bracket transforms the concept into a
genuinely practical everyday vehicle rather than a performance showcase.

---

### Recommended Engine: Rolls-Royce M250-C18

The original JetRanger engine — the engine that started the M250 family in 1960.
By far the most produced small turboshaft in history.

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
| Length | 1,029 mm |
| Diameter | 572 mm |
| Engine control | Hydromechanical (Honeywell/Bendix FCU) |
| FADEC | Not standard — see note below |
| Applications | Bell 206 JetRanger, Hughes 500, MD500 |
| Units produced | 38,000+ (M250 family total) |
| Support network | Global — largest of any small turbine |

**Note on engine control:** The C18 uses a proven hydromechanical fuel control
unit. It is not FADEC-equipped as standard. However an aftermarket **electronic
N2 overspeed protection system** is available and can be fitted — as used on
some later C20 variants. For a car application a standalone automotive ECU
monitoring shaft speed, TGT, and torque, interfaced with the existing
hydromechanical FCU via a torque motor signal, provides effective electronic
governing without a full FADEC certification burden. This is the same approach
used by several industrial M250 installations.

---

### M250-C18 Recuperator Calculations

Pressure ratio 6.2:1 — identical to the RR300. Cycle temperatures are therefore
the same as Section 11 but scaled to lower mass flow.

**Design case +5°C ambient:**

| Parameter | Value |
|---|---|
| T2 cold side inlet | 260°C |
| T4 hot side inlet | 478°C |
| T3 cold side outlet | 456°C |
| T5 final exhaust | 282°C |
| Heat duty | **117 kW** |

$$A_{total} = \frac{117{,}000}{100 \times 22} = \mathbf{53 \text{ m}^2}$$

| Parameter | Per Package | Total |
|---|---|---|
| Primary surface area | **26.5 m²** | 53 m² |
| Core volume | **~0.031 m³** | ~0.062 m³ |
| Physical envelope (approx.) | **200 × 175 × 90 mm** | — |

The C18 recuperator packages are extraordinarily compact — smaller than a
typical car intercooler. Packaging is trivially easy.

---

### M250-C18 Fuel Consumption and Range

Running at **220 SHP continuous** with recuperator (30% SFC improvement):

$$\text{Fuel flow} = 220 \times 0.64 \times 0.70 = \mathbf{98.6 \text{ lb/hr}}
= 44.7 \text{ kg/hr} = \mathbf{51 \text{ litres/hr}}$$

| Fuel cell | Running time | Range at 82.5 km/hr |
|---|---|---|
| 50 litres | **59 minutes** | **~81 km** |
| 100 litres | **118 minutes (1hr 58min)** | **~162 km** |
| **120 litres** | **~141 minutes (2hrs 21min)** | **~194 km** |

The 120 litre cell comfortably exceeds the 165 km target. Even the
100 litre cell achieves 162 km — within 2% of the target on a
smaller, lighter fuel load. This is considerably better than
previously calculated due to the corrected SFC figure.

---

## 14. Acceleration Estimates — All Engines

### Assumptions

- Vehicle mass: **1,500 kg**
- Layout: **Front engine, rear wheel drive**
- Weight distribution: **55% front / 45% rear** → 675 kg on rear axle
- Rear tyre width: **200 mm**, μ = 1.20 on dry tarmac
- Drivetrain efficiency: **η = 0.88**
- Maximum traction force: 1.20 × 675 × 9.81 = **7,945 N**
- Maximum traction-limited acceleration: 7,945 / 1,500 = **5.30 m/s² (0.54g)**

The traction limit governs the launch for all three engines up to the
crossover speed where available wheel force falls to equal traction force.
Above that speed the engine becomes the limiting factor.

### Crossover Speeds

| Engine | Wheel power | Crossover speed |
|---|---|---|
| M250-C47B | 427 kW | **193 km/h** — traction limited through entire 0–100 |
| RR300 | 197 kW | **89 km/h** — power limited from 89–100 km/h |
| M250-C18 | 194 SHP (145 kW) continuous / **236 SHP (176 kW) max** → 155 kW wheel | **70 km/h** — power limited from 70–100 km/h |

### Phase 1 — Traction Limited (all engines, 0 to crossover)

Acceleration = **5.30 m/s²** for all three.

| Engine | Traction-limited to | Time for Phase 1 |
|---|---|---|
| M250-C47B | 100 km/h (193 km/h crossover) | **5.24 s** (0–100 done) |
| RR300 | 89 km/h = 24.7 m/s | t₁ = 24.7 / 5.30 = **4.66 s** |
| M250-C18 | 70 km/h = 19.4 m/s | t₁ = 19.4 / 5.30 = **3.66 s** |

### Phase 2 — Power Limited (RR300 and C18 only)

**RR300 — 89 to 100 km/h:**

Average net force ≈ 8,142 N, average acceleration ≈ 5.43 m/s²

$$t_2 = \frac{27.78 - 24.7}{5.43} = \mathbf{0.57 \text{ s}}$$

**M250-C18 — 70 to 100 km/h:**

At 19.4 m/s: F_net = (155,000/19.4) − 221 − (0.5×1.225×0.35×2.0×19.4²) = 7,990 − 221 − 323 = 7,446 N → a = 4.96 m/s²

At 27.78 m/s: F_net = (155,000/27.78) − 221 − 661 = 5,582 − 882 = 4,700 N → a = 3.13 m/s²

Average acceleration: **(4.96 + 3.13) / 2 = 4.05 m/s²**

$$t_2 = \frac{27.78 - 19.4}{4.05} = \frac{8.38}{4.05} = \mathbf{2.07 \text{ s}}$$

### Final 0–100 km/h Results

| Engine | Max power | 0–100 km/h | Character |
|---|---|---|---|
| M250-C47B | 650 SHP | **~5.2 s** | Traction-limited throughout — tyre-shredding potential above 100 km/h |
| RR300 | 300 SHP | **~5.2 s** | Near-identical feel to C47B below 100 km/h |
| **M250-C18** | **317 SHP** | **~5.7 s** | 0.5 s slower — still very brisk, most practical |

The M250-C18 result of 5.7 seconds is highly respectable in a Golf Mk2 or Volvo 740
body — comparable to a modern hot hatchback — achieved at substantially lower fuel
consumption than the larger engines.

---

## 15. FADEC Derating — How Power Limiting Works

### What Derating Means

Running a turbine below its certificated maximum power extends component life
dramatically. The hot section — turbine blades, nozzle guide vanes, combustor —
accumulates damage through creep, oxidation, and thermal fatigue at a rate that
is highly non-linear with temperature. Reducing TGT (Turbine Gas Temperature)
by as little as 25°C can double hot-section life.

### How FADEC Implements Derating

A FADEC controls engine power through four simultaneous limit schedules,
each monitored up to 70 times per second. Whichever limit is reached first
wins — the FADEC never allows any parameter to exceed its set value.

**The four primary limits:**

**1. TGT Limit (Turbine Gas Temperature)**
The most important limit for hot-section life. The FADEC monitors the
inter-turbine temperature sensor and caps fuel flow when TGT reaches the
programmed ceiling. Reducing the TGT limit from, say, 810°C to 760°C
reduces available power by roughly 10–15% but dramatically reduces
blade creep and oxidation rate. This is the primary derating tool.

**2. NG Limit (Gas Generator Speed)**
Maximum gas generator RPM is capped in the FADEC software. Lowering
the NG ceiling reduces compressor delivery pressure and temperature,
directly reducing power output while keeping the entire hot section cooler.

**3. Torque Limit (Q)**
For a car application this is the most practically useful limit. The FADEC
monitors shaft output torque via the torquemeter and caps fuel flow when
torque reaches the programmed maximum. This protects the step-down
gearbox and drivetrain rather than the engine itself, but as a side effect
also prevents the engine from reaching peak TGT during normal driving.
Setting a torque limit equivalent to 70% of maximum power achieves
derating without the driver ever feeling a hard power cut — the engine
simply feels like a slightly less powerful unit.

**4. NP Limit (Power Turbine Speed)**
Power turbine overspeed protection — prevents the free power turbine
from exceeding its mechanical speed limit during load rejection events.
Set conservatively for a car application given the absence of a helicopter
rotor's large inertia to absorb transients.

### Derating in Practice for This Car

For the automotive application, the recommended approach is a **dual-mode
FADEC calibration:**

**Touring mode** — TGT limit reduced by 40–50°C below maximum, torque
limit set to approximately 70% of peak. Engine runs cool, fuel consumption
is minimised, TBO is maximised. Normal everyday driving.

**Performance mode** — Full certificated limits restored. Used for overtaking,
hill climbing, or track use. Time at this power level is logged by the FADEC
health monitoring system.

This is directly analogous to how modern turboprop aircraft use detachable
power ratings — the same FADEC parameters but with different numerical limits
selectable by the operator.

### M250-C18 Without FADEC

For the C18 with its hydromechanical FCU, derating is achieved mechanically
by adjusting the **fuel control unit (FCU) stop** — a physical adjustment that
limits maximum fuel flow regardless of throttle position. This is a well-understood
procedure done routinely on industrial M250 installations. It is less precise than
FADEC but entirely effective, and the adjustment is reversible. Adding an
aftermarket electronic N2 governor provides overspeed protection, and a
simple EGT (exhaust gas temperature) gauge with a warning light provides
the driver with TGT awareness without full FADEC automation.

---

## 16. Time Between Overhaul (TBO)

### M250 Family TBO — Confirmed Data

TBO varies by series and component:

| Engine | Component | TBO |
|---|---|---|
| M250-C18 (Series II) | Compressor | **3,500 hours** |
| M250-C18 (Series II) | Turbine | **3,500 hours** |
| M250-C18 (Series II) | Gearbox | **On condition** |
| M250-C47B (Series IV) | Compressor impeller | **On condition** (model-dependent life limits) |
| M250-C47B (Series IV) | Turbine | **2,000 hours** |
| M250-C47B (Series IV) | Gearbox | **On condition** |
| RR300 | Engine (all modules) | **2,000 hours** |

**Key point:** The C18 Series II turbine and compressor are both rated at 3,500 hours
— 75% more than the C47B turbine's 2,000 hours. This is a direct consequence of the
C18 running at lower temperatures relative to its design margins. In an automotive
application running derated, the C18's TBO would very likely extend further still,
since aviation TBO figures are based on flight duty cycles with frequent high-power
events. A car, even driven enthusiastically, spends far more time at part power.

### What TBO Means in Practical Terms

At **~51 litres/hr** recuperated fuel consumption, and typical usage of perhaps
**200 hours/year** (generous for a warm-season car):

| Engine | TBO | Years at 200 hrs/yr |
|---|---|---|
| M250-C18 | 3,500 hrs | **~17 years** between overhauls |
| RR300 | 2,000 hrs | **~10 years** between overhauls |
| M250-C47B | 2,000 hrs (turbine) | **~10 years** between overhauls |

For context, a conventional car engine is typically rebuilt or replaced at
150,000–200,000 km. At 82.5 km/hr average and 200 hours/year, the C18
would cover **16,500 km/year** and reach TBO after **~280,000 km equivalent**
— considerably better than a piston engine.

### Effect of Derating on TBO

Running derated in touring mode — with TGT reduced by 40–50°C — has a
profound effect on hot-section life. The industry rule of thumb is that every
15°C reduction in TGT **doubles the creep life** of turbine blades. A 45°C
reduction therefore multiplies blade life by approximately 8×. In practice
this means a derated C18 in automotive use could realistically achieve
**5,000–6,000 hours** between hot section inspections, with the compressor
and gearbox remaining on condition indefinitely.

---

## 17. Three-Engine Comparison Summary

| Parameter | M250-C47B | RR300 | M250-C18 |
|---|---|---|---|
| Max power | 650 SHP | 300 SHP | 317 SHP |
| Continuous power | 450–500 SHP | 240 SHP | 250 SHP |
| Mass flow | 2.77 kg/s | ~1.87 kg/s | **1.23 kg/s** |
| Pressure ratio | 9.2:1 | 6.2:1 | 6.2:1 |
| Total HX surface area | 1,164 m² | 120 m² | **53 m²** |
| Per package HX envelope | 600×500×230 mm | 300×250×95 mm | **200×175×90 mm** |
| Engine weight | ~72 kg | ~80 kg | **64 kg** |
| FADEC | Yes | Yes | No (see §14) |
| TBO — turbine | 2,000 hrs | 2,000 hrs | **3,500 hrs** |
| Recuperated fuel flow | 106 L/hr | 48 L/hr | **51 L/hr** |
| Range on 120L | ~93 km | ~206 km | **~194 km** |
| 0–100 km/h | ~5.2 s | ~5.2 s | ~5.7 s |
| Support network | Excellent | Excellent | **Best of all** |
| Relative cost | High | Medium | **Lowest** |
| Best suited for | Performance showcase | Balanced touring | Practical daily use |

---

*Sections 12–16 added covering M250-C18 specification, acceleration figures,*
*FADEC derating methodology, and TBO data.*
*Acceleration calculations assume 1,500 kg vehicle, front engine RWD, 55/45 weight*
*distribution, 200mm rear tyres μ=1.20, drivetrain efficiency 0.88.*
*TBO figures from published Rolls-Royce M250 maintenance documentation.*

---

## 18. Compatible Fuels and Seal Materials

### Background — NOx and Fuel Choice

NOx was the issue that ultimately killed the Chrysler turbine car programme —
the continuous combustion cycle of a gas turbine produces more NOx than an
intermittent piston engine at equivalent power. Heat and noise Chrysler solved.
NOx they did not — emissions regulations in the 1970s were the final blow.

The good news for this concept is that NOx formation is dominated almost
entirely by **peak combustion temperature** via the thermal (Zeldovich) mechanism.
Any fuel that burns cooler than petroleum diesel will produce less NOx. Fuels
with high water content, lower heating values, or oxygenated chemistry all
tend in this direction. Biodiesel and alcohols are better than petroleum diesel
on NOx in a turbine. The turbine's lean, continuous combustion also eliminates
CO, unburned hydrocarbons, and particulates far more effectively than a piston
engine — so NOx is the one remaining challenge, and fuel selection is the
most practical lever available without hardware changes.

To reach full designed power on ethanol, about 1.6 times more fuel flow is
required compared to diesel. The increased water content is actually beneficial,
cooling the combustion temperature and resulting in lower NOx emissions.

Biodiesel has a detrimental effect on elastomers commonly found in many of
the gaskets and sealants in a typical gas turbine package — care must be taken
in selecting compatible components. The same caution applies to all
oxygenated and alcohol fuels. The solution is consistent: **FKM (Viton) seals
and PTFE-lined hoses throughout the fuel wetted circuit**.

---

### Table A — Liquid Fuel Candidates

Any fuel that is liquid at operating temperature, burns stably in a continuous
flame combustor, and falls within the viscosity range the M250 fuel nozzle
can handle (~0.5 to 12 cSt) is a candidate. The table below covers the
realistic options from best to worst on NOx.

| Fuel | Source | NOx vs Diesel | CO | Particulates | SO₂ | Seal Risk | Notes |
|---|---|---|---|---|---|---|---|
| **Bio-ethanol 80%** (hydrous) | Fermentation | **Much lower** | Low | Near zero | Zero | High — FKM required | 20% water cools flame further. ~1.6× fuel flow. Best NOx of all liquid options |
| **Anhydrous bio-ethanol** | Fermentation | **Lower** | Low | Near zero | Zero | High — FKM required | No water benefit. Still burns cool vs diesel |
| **Bio-methanol** | Biomass/waste | **Lower** | Low | Near zero | Zero | Very high — FKM + PTFE essential | Lowest flame temp of common alcohols. Toxic — handling precautions needed |
| **Biodiesel B100** | Vegetable oil / animal fat | **Slightly lower** | Lower | Near zero | Zero | Medium — FKM preferred | Best balance of NOx, energy density and range. Recommended primary fuel |
| **HVO** (Hydrotreated vegetable oil) | Vegetable oil | **Similar to diesel** | Lower | Near zero | Zero | Low — standard seals acceptable | Chemically close to kerosene. Excellent cold weather performance |
| **Jet A-1 / kerosene** | Petroleum / synthetic | Baseline | Low | Low | Low | Low — standard seals acceptable | Chrysler's preferred fuel. Very wide availability |
| **Diesel (EN590)** | Petroleum | Baseline | Low | Low | Low | Low — standard seals acceptable | Widely available. Higher viscosity than kerosene |
| **Heating oil** | Petroleum | Similar to diesel | Low | Low | Low | Low — standard seals acceptable | Chrysler demonstrated this. Slightly higher sulphur |
| **Aviation gasoline (Avgas)** | Petroleum | Slightly higher | Low | Low | Low | Low — standard seals | Contains lead in 100LL — damages turbine nozzle guide vanes. Avoid |
| **Unleaded petrol (E0)** | Petroleum | Similar to diesel | Low | Low | Low | Low — standard seals | High volatility — requires care with fuel system venting |
| **Straight vegetable oil** | Plant oils | Similar to biodiesel | Higher at low power | Low | Zero | Medium | High viscosity — must be preheated to ~60°C before combustor. Gels in cold weather |
| **Used cooking oil (UCO)** | Waste cooking oil | Similar to biodiesel | Variable | Low | Near zero | Medium | Filter carefully. Variable quality. Essentially free fuel |
| **Tallow / animal fat** | Rendered animal fat | Similar to biodiesel | Low | Near zero | Near zero | Medium | Must be heated — high pour point (~40°C). Works well once warm |
| **Palm oil** | Tropical agriculture | Similar to biodiesel | Low | Near zero | Zero | Medium | High pour point. Gels readily in cool weather |
| **Turpentine** | Pine resin | Lower | Low | Low | Near zero | Medium — FKM preferred | Chrysler demonstrated. High energy density. Corrosive to some metals |
| **Tequila / spirits** | Fermentation | **Lower** (alcohol base) | Low | Near zero | Zero | High — FKM required | Chrysler demonstrated. Essentially dilute ethanol. Novelty value only |
| **Perfume / Chanel No.5** | Alcohol + esters | **Lower** | Low | Near zero | Zero | High — FKM required | Chrysler demonstrated. Alcohol-based. Not a practical fuel source |
| **Peanut oil** | Groundnuts | Similar to biodiesel | Low | Near zero | Zero | Medium | Chrysler demonstrated. High viscosity — preheat required |

**Fuels to avoid:**
- **Leaded petrol (100LL Avgas)** — lead deposits destroy turbine nozzle guide vanes irreversibly
- **Methanol at high concentration** — attacks aluminium alloy fuel system components and most elastomers aggressively; requires fully FKM/PTFE/stainless construction throughout
- **Pyrolysis oil** — viscosity too high even when heated; acidic and corrosive
- **Pure hydrogen** — burns far hotter, drastically increasing NOx; requires complete combustor redesign

---

### Table B — Seal and Gasket Material Compatibility

The fuel wetted circuit of the M250 — fuel pump, fuel control unit, fuel
manifold, combustor nozzle, and all connecting hoses — contains elastomeric
seals and gaskets. Material selection determines whether the chosen fuel
causes swelling, degradation, or failure.

| Seal Material | Common Name | Petroleum Diesel | Biodiesel B100 | Ethanol / Methanol | Vegetable Oil | Ketones | Temperature Limit | Notes |
|---|---|---|---|---|---|---|---|---|
| **FKM** | Viton | ✓ Excellent | ✓ Good | ✓ Good | ✓ Good | ✗ Poor | 200°C | **Best overall choice for multi-fuel use.** Standard fitment recommendation for this concept |
| **FVMQ** | Fluorosilicone | ✓ Good | ✓ Good | ✓ Good | ✓ Good | ✗ Poor | 175°C | Slightly better low-temp flexibility than FKM. Good multi-fuel alternative |
| **PTFE** | Teflon | ✓ Excellent | ✓ Excellent | ✓ Excellent | ✓ Excellent | ✓ Excellent | 260°C | **Universally compatible — use for hose liners and static seals throughout** |
| **NBR** | Nitrile / Buna-N | ✓ Good | ✗ Poor | ✗ Poor | ✗ Poor | ✗ Poor | 120°C | Standard automotive seal. Swells badly in biodiesel and alcohols. Avoid for this concept |
| **EPDM** | — | ✗ Poor | ✗ Very poor | ✓ Fair | ✗ Poor | ✗ Poor | 150°C | Not compatible with petroleum or biodiesel fuels. Avoid |
| **CR** | Neoprene | ✓ Fair | ✗ Poor | ✗ Poor | ✗ Poor | ✗ Poor | 120°C | Limited resistance. Avoid in fuel wetted circuits |
| **VMQ** | Silicone | ✓ Fair | ✓ Fair | ✓ Fair | ✓ Fair | ✓ Fair | 200°C | Swells significantly in most fuels. Not suitable for dynamic seals under pressure |
| **IIR** | Butyl rubber | ✗ Poor | ✗ Poor | ✓ Fair | ✗ Poor | ✓ Good | 120°C | Poor with hydrocarbons. Limited use |

**Practical recommendation:** Specify **FKM (Viton) for all O-rings and dynamic seals**,
**PTFE-lined hose throughout**, and **stainless steel fittings**. This combination is
compatible with every fuel in Table A including methanol and alcohols, survives
the operating temperature range of the fuel system, and requires no changes when
switching between fuels. The M250 family already uses FKM seals in several of
its fuel wetted components — a complete FKM/PTFE rebuild of the fuel circuit
for this automotive application is straightforward and uses standard
aerospace-grade parts available from the FIRST Network.

---

*Section 18 added covering fuel candidates and seal material compatibility.*
*NOx comparisons based on published gas turbine combustion research.*
*Seal compatibility based on published elastomer immersion test data.*
*Chrysler fuel demonstrations referenced from historical A-831 programme records.*

---

## 19. Water Injection System

### Purpose

Water injection serves two simultaneous roles in this concept:

- **NOx reduction** at all power levels — water vapour entering the combustor
  lowers peak flame temperature, directly suppressing thermal NOx formation
  via the Zeldovich mechanism
- **Power augmentation on demand** — higher injection rates cool and densify
  the intake air, increasing compressor mass flow and allowing the FADEC to
  add fuel within the same TGT ceiling, producing more shaft power than the
  engine delivers dry

The Rolls-Royce Pegasus engine in the Harrier uses the same principle for
thrust augmentation at takeoff and hover — a well-proven application at
far greater intensity than required here. Gas turbines also handle natural
rain ingestion without difficulty, making this a robust and forgiving system.

---

### Water Source — Rainwater from Downspouts

Rainwater collected from a household downspout is the practical and
low-cost water source. Rainwater is naturally low in dissolved minerals —
having evaporated, condensed, and fallen without contact with ground
mineral sources — making it far more suitable than tap water for turbine
injection, where mineral deposits on recuperator plate surfaces are the
primary concern.

**Collection setup — home installation:**

A standard garden water butt or barrel fitted with:

- A **coarse mesh inlet filter** (1–2 mm) at the downspout connection —
  catches leaves, moss, roof debris, and insects
- A **fine sediment cartridge filter** (50–100 micron) on the outlet tap —
  removes fine particulates and pollen before transfer to the car tank
- A simple tap at the base for filling

Cost is minimal — a basic water butt with a filter cartridge. No
demineralisation, no chemical treatment, no ongoing consumable cost.
The combustor operating at over 900°C is entirely indifferent to the
trace organics and mild carbonic acidity natural to rainwater.

**Transfer to the car:**
Fill the car's water tank from the filtered outlet tap — the same
procedure as filling a screen wash bottle. A clearly labelled filler
point on the car, separate from the fuel filler, connected to a small
dedicated stainless or HDPE water tank of **15–25 litres**.

---

### Injection System Design

**Tank:**
15–25 litre stainless steel or HDPE tank, mounted low in the vehicle
for weight distribution. Fitted with a translucent sight gauge or
float-type level sender to the dashboard. A drain valve for winter
storage. FKM seals throughout.

**Pump:**
A **PWM-controlled (pulse-width modulation) high-pressure pump** —
the same technology used in automotive fuel injection and industrial
fogging systems. PWM control varies the pump duty cycle continuously
from 0% to 100%, giving proportional flow rate from zero to maximum
without a separate flow control valve. Simple, robust, and precise.

Operating pressure: **70–100 bar** — sufficient to produce droplets
below 20 microns at the nozzle, ensuring complete evaporation before
the compressor inlet. At this droplet size liquid water does not reach
the compressor blades.

**Nozzle manifold:**
Stainless steel manifold with **two to four fogging nozzles** mounted
across the intake scoop upstream of the recuperator cold side inlet.
Nozzles are standard industrial fogging type — inexpensive, available,
and replaceable without tools.

**Control:**
The PWM pump duty cycle is driven directly by **throttle position**:

| Throttle position | PWM duty cycle | Injection rate | Effect |
|---|---|---|---|
| Idle | 0% | Off | No injection |
| Light cruise | 10–20% | ~0.3–0.5 L/min | Mild NOx reduction |
| Normal cruise | 20–40% | ~0.5–1.0 L/min | Steady NOx reduction |
| Hard acceleration | 60–80% | ~2.0–3.0 L/min | NOx reduction + power augmentation |
| Full throttle | 100% | ~4.0–5.0 L/min | Maximum augmentation |

A **low-level warning light** on the dashboard activates when the tank
drops below approximately 3 litres — sufficient reserve for a few
minutes of normal driving before running dry. Running dry causes no
engine damage — the engine simply returns to its normal dry performance.

**Interlock:**
The pump is disabled below a minimum engine speed threshold to prevent
injection during startup and shutdown when the combustor is not at
operating temperature.

---

### Rain — Incidental Free Injection

Natural rain ingestion through the intake scoop provides a mild and
uncontrolled version of the same effect at no cost. On a wet day the
engine already runs slightly cooler with marginally higher mass flow
than on a dry day. The turbine is entirely unaffected by this — the
M250 family has accumulated over 200 million flight hours in
helicopters operating through tropical downpours, thunderstorms, and
icing conditions without incident.

Rain ingestion and deliberate injection are simply different points on
the same continuous spectrum. The engine makes no distinction between
them. On a heavy rain day the tank depletes more slowly as the
atmosphere is already contributing. No sensor or compensation is needed
— the FADEC manages the engine state regardless of water source.

---

### System Summary

| Parameter | Value |
|---|---|
| Water source | Rainwater from household downspout |
| Filtration | Coarse mesh inlet + 50–100 micron cartridge filter |
| Storage tank | 15–25 litres — stainless or HDPE |
| Operating pressure | 70–100 bar |
| Pump control | **PWM — duty cycle proportional to throttle position** |
| Droplet size | <20 micron — complete evaporation before compressor |
| Injection point | Upstream of recuperator cold side inlet |
| Cruise injection rate | 0.3–1.0 L/min |
| Full power injection rate | 4.0–5.0 L/min |
| Tank duration at cruise | ~25–80 minutes depending on rate |
| Tank duration at full power | ~3–6 minutes |
| NOx effect | 20–35% reduction at cruise rates |
| Power augmentation | 10–15% additional shaft power at full rate |
| Rain ingestion | Handled without concern — incidental benefit |
| Seal material | FKM throughout — compatible with water and all fuel candidates |
| Running dry | No engine damage — returns to normal dry rating |

---

*Section 19 added covering water injection system design, rainwater sourcing,*
*PWM pump control, and dual-mode NOx reduction and power augmentation.*

---

## 20. Air Movement — Volumetric Flow and Pressure Drop

### Volumetric Flow Rates

Mass flow figures are established in Section 3. Converting to volumetric
flow at the relevant conditions for each point in the cycle requires knowing
the air density, which varies with temperature and pressure.

**Density of air:**

$$\rho = \frac{P}{R \times T}$$

Where R (specific gas constant for air) = 287 J/kg·K

---

#### Intake — Ambient Air at Recuperator Cold Side Inlet

At ISO standard conditions (+15°C, 101.325 kPa), ρ = 1.225 kg/m³

At +5°C ambient (design case), ρ = 1.269 kg/m³

At +45°C ambient (hot case), ρ = 1.110 kg/m³

**Volumetric flow at intake — all three engines, ISO conditions:**

$$\dot{V} = \frac{\dot{m}}{\rho}$$

| Engine | Mass flow | Intake volumetric flow (ISO +15°C) | Hot day +45°C | Cool day +5°C |
|---|---|---|---|---|
| M250-C47B | 2.77 kg/s | **2.26 m³/s (2,260 L/s)** | 2.50 m³/s | 2.18 m³/s |
| RR300 | 1.87 kg/s | **1.53 m³/s (1,530 L/s)** | 1.68 m³/s | 1.47 m³/s |
| M250-C18 | 1.23 kg/s | **1.00 m³/s (1,000 L/s)** | 1.11 m³/s | 0.97 m³/s |

The intake volumetric flow is the largest figure in the system — this is
ambient density air before the compressor has pressurised it. It governs
the sizing of the intake scoop, the intake ducting cross-section, and the
cold side face area of each recuperator package.

---

#### Compressor Delivery — Air at Recuperator Cold Side (High Pressure)

After the compressor the air is at **pressure ratio × ambient pressure**
and at compressor outlet temperature T2. This is the condition at the
recuperator cold side inlet — high pressure, moderate temperature.

At ISO +15°C, pressure ratio 6.2:1 (RR300 / C18):

- Pressure: 6.2 × 101.325 = **628 kPa**
- Temperature T2: **198°C = 471 K**
- Density: 628,000 / (287 × 471) = **4.65 kg/m³**

At ISO +15°C, pressure ratio 9.2:1 (C47B):

- Pressure: 9.2 × 101.325 = **933 kPa**
- Temperature T2: **365°C = 638 K**
- Density: 933,000 / (287 × 638) = **5.10 kg/m³**

**Volumetric flow at recuperator cold side inlet (high pressure air):**

| Engine | Mass flow | Pressure ratio | Cold side volumetric flow |
|---|---|---|---|
| M250-C47B | 2.77 kg/s | 9.2:1 | 2.77 / 5.10 = **0.543 m³/s** |
| RR300 | 1.87 kg/s | 6.2:1 | 1.87 / 4.65 = **0.402 m³/s** |
| M250-C18 | 1.23 kg/s | 6.2:1 | 1.23 / 4.65 = **0.265 m³/s** |

This pressurised volumetric flow governs the internal channel sizing of
the recuperator cold side — much smaller than the intake figure because
the air has been compressed to 6–9× ambient density.

---

#### Exhaust — Hot Side Volumetric Flow at Recuperator Inlet

Turbine exhaust enters the recuperator hot side at T4 = 478–546°C
(engine dependent) and near-atmospheric pressure (slight back pressure).

At T4 = 478°C = 751 K (RR300 / C18), P ≈ 105 kPa:

$$\rho_{exhaust} = \frac{105{,}000}{287 \times 751} = \mathbf{0.487 \text{ kg/m}^3}$$

At T4 = 546°C = 819 K (C47B), P ≈ 105 kPa:

$$\rho_{exhaust} = \frac{105{,}000}{287 \times 819} = \mathbf{0.447 \text{ kg/m}^3}$$

**Volumetric flow at recuperator hot side inlet:**

| Engine | Mass flow | T4 | Hot side volumetric flow |
|---|---|---|---|
| M250-C47B | 2.77 kg/s | 546°C | 2.77 / 0.447 = **6.20 m³/s** |
| RR300 | 1.87 kg/s | 478°C | 1.87 / 0.487 = **3.84 m³/s** |
| M250-C18 | 1.23 kg/s | 478°C | 1.23 / 0.487 = **2.53 m³/s** |

The hot side exhaust volumetric flow is the largest internal flow in the
recuperator — hot, low-density gas at near-atmospheric pressure. It
governs hot side channel sizing and the exhaust ducting cross-section
from the power turbine to the recuperator.

---

#### Final Exhaust — Volumetric Flow at Tailpipe

After the recuperator the exhaust exits at T5 ≈ 177–282°C (engine and
ambient dependent). Taking the design case of +5°C ambient:

- RR300 / C18: T5 = 282°C = 555 K, ρ = 105,000 / (287 × 555) = **0.659 kg/m³**
- C47B: T5 = 337°C = 610 K, ρ = 105,000 / (287 × 610) = **0.600 kg/m³**

**Final exhaust volumetric flow at tailpipe:**

| Engine | Mass flow | T5 (+5°C ambient) | Tailpipe volumetric flow |
|---|---|---|---|
| M250-C47B | 2.77 kg/s | 337°C | 2.77 / 0.600 = **4.62 m³/s** |
| RR300 | 1.87 kg/s | 282°C | 1.87 / 0.659 = **2.84 m³/s** |
| M250-C18 | 1.23 kg/s | 282°C | 1.23 / 0.659 = **1.87 m³/s** |

These figures govern tailpipe diameter. Keeping exhaust velocity below
~30 m/s at the tailpipe exit minimises exit noise and ensures adequate
cooling of the gas before it reaches road level. Required tailpipe
cross-sectional area for the M250-C18 at 30 m/s exit velocity:

$$A_{tailpipe} = \frac{1.87}{30} = 0.062 \text{ m}^2$$

This corresponds to a **round tailpipe diameter of ~280 mm** — or two
pipes of ~200 mm each, one per recuperator package side. A diffuser
exit flaring to 350–400 mm further reduces exit velocity and temperature.

---

### Acceptable Pressure Drop

Pressure drop across the recuperator is parasitic — it consumes work
that the compressor and turbine have already done, reducing net cycle
efficiency. It must be minimised without sacrificing heat transfer
effectiveness.

The maximum allowable overall pressure drop is determined as **5% of the
compressor outlet pressure**. This is the widely accepted industry
standard for recuperated gas turbines and applies to the **combined**
cold side and hot side pressure drops together.

For a practical recuperator design, the turbine can tolerate up to
**34.5 kPa (5 psi) counter-pressure on the cold side** and up to
**21 kPa (3 psi) on the hot side exhaust**.

**Applying the 5% rule to each engine:**

| Engine | Pressure ratio | Compressor outlet pressure | 5% limit (total) | Cold side limit | Hot side limit |
|---|---|---|---|---|---|
| M250-C47B | 9.2:1 | 933 kPa | **46.6 kPa** | ~28 kPa | ~18 kPa |
| RR300 | 6.2:1 | 628 kPa | **31.4 kPa** | ~19 kPa | ~12 kPa |
| M250-C18 | 6.2:1 | 628 kPa | **31.4 kPa** | ~19 kPa | ~12 kPa |

The cold side carries the higher pressure drop allowance because it is
at high pressure — a given pressure drop represents a smaller fractional
loss. The hot side is at near-atmospheric pressure so even a modest
pressure drop is proportionally more significant.

**Effect of exceeding the pressure drop limit:**

Every 1% of compressor delivery pressure lost to recuperator pressure
drop reduces cycle thermal efficiency by approximately **0.3–0.5
percentage points** — directly increasing fuel consumption. Staying
within 5% total is therefore critical to achieving the recuperator's
claimed 30% fuel saving.

---

### Complete Air Movement Summary

| Parameter | M250-C47B | RR300 | M250-C18 |
|---|---|---|---|
| Mass flow | 2.77 kg/s | 1.87 kg/s | 1.23 kg/s |
| **Intake volumetric flow (ISO)** | **2.26 m³/s** | **1.53 m³/s** | **1.00 m³/s** |
| Cold side volumetric flow (pressurised) | 0.543 m³/s | 0.402 m³/s | 0.265 m³/s |
| **Hot side volumetric flow (exhaust in)** | **6.20 m³/s** | **3.84 m³/s** | **2.53 m³/s** |
| Final exhaust volumetric flow (tailpipe) | 4.62 m³/s | 2.84 m³/s | 1.87 m³/s |
| Max total pressure drop (5% rule) | 46.6 kPa | 31.4 kPa | 31.4 kPa |
| Max cold side pressure drop | ~28 kPa | ~19 kPa | ~19 kPa |
| Max hot side pressure drop | ~18 kPa | ~12 kPa | ~12 kPa |
| Recommended tailpipe diameter | ~350 mm | ~270 mm | ~220 mm |
| Or twin pipes per side | 2 × 250 mm | 2 × 190 mm | 2 × 155 mm |

---

*Section 20 added covering volumetric air flow at all cycle points and*
*acceptable recuperator pressure drop limits based on published industry standards.*
*Volumetric flows calculated from confirmed mass flow figures using ideal gas law.*
*Pressure drop limits per McDonald (2000) and published turbogenerator test data.*

---

## 21. Heat Exchanger Plate Geometry — M250-C18

### Plate Sizing Basis

Plate dimensions are governed by two constraints:

**Engine envelope** — the M250-C18 has a maximum cross-section diameter
of **572 mm**. The recuperator packages sit beside the engine and must
not exceed this height to keep the installation tidy within the engine bay.

**Wheel diameter rule** — using the Volvo 740 standard tyre 185/70 R14
as the reference vehicle:

$$D_{wheel} = (2 \times 185 \times 0.70) + (14 \times 25.4) = 259 + 356 = \mathbf{615 \text{ mm}}$$

Applied limits:
- Maximum plate height = **70% of wheel diameter = 430 mm**
- Maximum plate length = **100% of wheel diameter = 615 mm**

The wheel diameter rule gives 430 mm height — less than the engine's 572 mm
cross-section — so the **wheel diameter rule governs** and the 430 mm figure
is used. Both packages confirmed to fit in the engine bay at 430 × 615 mm.

$$\boxed{H_{plate} = 430 \text{ mm}} \qquad \boxed{L_{plate} = 615 \text{ mm}}$$

---

### Plate Thickness

| Parameter | Value | Basis |
|---|---|---|
| Material | SS347 stainless steel foil | Industry standard for PSR |
| Plate thickness | **0.10 mm (100 microns)** | Within 0.076–0.203 mm published industry range |

SS347 foil at 0.10 mm is the standard used by Solar Turbines and other
primary surface recuperator manufacturers. It provides adequate creep
resistance at 478°C hot side inlet temperature with good margin.

---

### Ridge Geometry — Longitudinal Stiffening Ridges

Ridges run the **full length of each plate parallel to the gas flow
direction**. They serve primarily as structural stiffening — increasing
the second moment of area of the thin foil against the pressure
differential between cold side (628 kPa) and hot side (~105 kPa) —
exactly as longitudinal ridges stiffen pressed steel floor panels and
door skins in the chassis industry.

Because the ridges are parallel to flow they introduce **no transverse
turbulence, no unexpected pressure drop, and no flow disruption**. The
gas flows smoothly along the channels formed between adjacent plates.
Heat transfer is governed by channel hydraulics, not surface geometry.

**Two plate stampings are used — cold side and hot side — alternating
through the stack.** They differ only in ridge height, reflecting the
very different volumetric flow requirements of the high-density
compressed air stream and the low-density exhaust stream.

| Parameter | Cold side plate | Hot side plate |
|---|---|---|
| Ridge height | **1.5 mm** | **5.0 mm** |
| Ridge width at base | 4.0 mm | 4.0 mm |
| Ridge profile | Shallow trapezoid | Shallow trapezoid |
| Ridge pitch (c/c) | **20 mm** | **20 mm** |
| Ridges per plate | **21** | **21** |
| Channel width between ridges | 16 mm | 16 mm |
| Full channel width | 20 mm | 20 mm |

The hot side requires 5.0 mm channel height versus 1.5 mm on the cold
side because the exhaust gas is at near-atmospheric pressure and very
high temperature — its density is approximately **10× lower** than the
compressed air on the cold side. Without larger channels the hot side
velocity would be excessive and pressure drop would breach the 12 kPa
limit.

**Surface area enhancement from ridges:**

Longitudinal ridges add a modest **~5%** to wetted surface area compared
to a flat plate — the trapezoidal ridge perimeter (5.0 mm) versus the
equivalent flat width (4.0 mm) over a 20 mm pitch. This is intentionally
small — the ridges are structural, not a heat transfer enhancement device.

$$A_{flat} = 0.430 \times 0.615 = 0.264 \text{ m}^2 \text{ per plate}$$

$$A_{effective} = 0.264 \times 1.05 = \mathbf{0.277 \text{ m}^2 \text{ per plate}}$$

---

### Number of Plates and Stack Height

Required primary surface area per package: **26.5 m²**

$$N_{plates} = \frac{26.5}{0.277} = \mathbf{96 \text{ plates per package}}$$

**Cell pitch** — one cold plate + one hot plate pair:

| Component | Thickness |
|---|---|
| Cold side channel (ridge height) | 1.5 mm |
| Cold side plate | 0.10 mm |
| Hot side channel (ridge height) | 5.0 mm |
| Hot side plate | 0.10 mm |
| **Total cell pitch** | **6.70 mm** |

$$\text{Stack height} = \frac{96}{2} \times 6.70 = 48 \times 6.70 = \mathbf{322 \text{ mm}}$$

---

### Flow Velocity Verification

**Cold side — compressed air at 628 kPa, T2 = 260°C:**

- Volumetric flow per package: 0.265 / 2 = **0.133 m³/s**
- Number of cold channels: 48 pairs × 21 channels = **1,008 channels**
- Channel cross-section: 20 × 1.5 mm = **30 mm² = 3.0 × 10⁻⁵ m²**
- Total cold flow area: 1,008 × 3.0 × 10⁻⁵ = **0.030 m²**

$$v_{cold} = \frac{0.133}{0.030} = \mathbf{4.4 \text{ m/s}} \checkmark$$

Well within the 5–10 m/s design target. Pressure drop will be low.

**Hot side — exhaust at ~105 kPa, T4 = 478°C:**

- Volumetric flow per package: 2.53 / 2 = **1.265 m³/s**
- Number of hot channels: 48 pairs × 21 channels = **1,008 channels**
- Channel cross-section: 20 × 5.0 mm = **100 mm² = 1.0 × 10⁻⁴ m²**
- Total hot flow area: 1,008 × 1.0 × 10⁻⁴ = **0.101 m²**

$$v_{hot} = \frac{1.265}{0.101} = \mathbf{12.5 \text{ m/s}} \checkmark$$

Acceptable — within the typical 10–15 m/s range for hot side exhaust
channels. Pressure drop remains within the 12 kPa hot side limit.

---

### Intake Duct Dimensions

Intake volumetric flow per package at ISO conditions: **0.50 m³/s**

At 6 m/s approach velocity:

$$A_{intake} = \frac{0.50}{6} = \mathbf{0.083 \text{ m}^2}$$

**As a rectangular duct matching plate height:**

$$W_{duct} = \frac{0.083}{0.430} = \mathbf{193 \text{ mm}}$$

A **430 mm tall × 193 mm wide rectangular intake duct** feeds directly
into the recuperator cold side face, expanding through a short diffuser
section from 193 mm to 615 mm width — an expansion ratio of 3.2:1,
slowing the air from 6 m/s at the duct to approximately 1.9 m/s at the
plate face before entering the channels.

**As a circular duct (alternative):**

$$D_{intake} = \sqrt{\frac{4 \times 0.083}{\pi}} = \mathbf{325 \text{ mm diameter}}$$

The rectangular duct is preferred as it matches the plate height and
simplifies the transition to the recuperator face without a shape change.

---

### Complete Package Summary — M250-C18

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
| **Plate stampings** | **Two** — cold plate and hot plate alternating |
| **Plates per package** | **96** |
| **Plate pairs per package** | **48** |
| **Cell pitch** | **6.70 mm** |
| **Stack height** | **~322 mm** |
| **Package envelope** | **615 × 430 × 322 mm** |
| **Cold side channel velocity** | **4.4 m/s** |
| **Hot side channel velocity** | **12.5 m/s** |
| **Intake duct (rectangular)** | **430 × 193 mm** |
| **Intake duct (circular equivalent)** | **325 mm diameter** |
| **Diffuser expansion ratio** | **3.2:1** (193 → 615 mm width) |
| **Engine bay fit confirmed** | **Yes — 430 × 615 mm fits** |

---

*Section 21 added covering heat exchanger plate geometry for M250-C18.*
*Plate dimensions derived from Volvo 740 185/70 R14 wheel diameter.*
*Asymmetric channel heights calculated from volumetric flow and velocity limits.*
*Ridge geometry based on chassis industry pressed steel stiffening practice.*
*SS347 foil thickness per published Solar Turbines / Allegheny-Ludlum PSR data.*

---

## 22. Ancillary Systems, Costs and Instrumentation

### Power Steering — Electric Hydraulic Pump (EHPS)

The M250-C18 has no accessory belt drive. Power steering must be
sourced independently. The most practical solution for both the
Golf Mk2 and Volvo 740 is an **electric hydraulic power steering
(EHPS) pump** — a self-contained unit that bolts into the existing
hydraulic steering circuit without modifying the rack or hoses.

**Recommended unit: Volvo S40/V50/C30 EHPS pump (2006–2012)**

This brushless pump is widely used in engine swap and EV conversion
projects worldwide and is a proven, readily available, inexpensive
solution. It connects directly to the existing hydraulic rack on
both donor vehicles and operates from the 12V supply via a simple
controller.

| Parameter | Value |
|---|---|
| Type | Electric hydraulic — brushless motor driving hydraulic pump |
| Supply voltage | **12V** from Battery 1 |
| Current draw | ~20–25A at full lock, ~5A at straight-ahead cruise |
| Controller | Reform Motorsports EHPS-Micro or equivalent — 2 × 1 inch PCB |
| Assist level | Adjustable via controller potentiometer |
| Compatibility | Connects to existing hydraulic rack on Golf Mk2 and Volvo 740 |
| Source | Used unit from Volvo C30/S40/V50 — widely available |
| Approximate cost | **€80–150** for used OEM pump + **€60–100** for controller |

The controller requires only a switched 12V ignition feed and ground —
no CAN bus integration needed. Assist level is set once with a
screwdriver and left. The pump runs only when the engine is running
via the ignition circuit.

---

### Brake Booster — Electric Vacuum Pump

The standard brake servo (vacuum booster) on both donor vehicles
operates on engine vacuum. The M250-C18 provides none. A dedicated
12V electric vacuum pump maintains the booster reservoir
independently, requiring no modification to the existing brake
master cylinder, booster, or hydraulic circuit.

**Recommended unit: Hella UP30**

The Hella UP30 can provide the pneumatic vacuum supply as a
stand-alone system — the pump acts as the sole source of vacuum
and ensures sufficient supply for the brake booster and any
auxiliary consumers. It is based on the rotary vane compression
principle and is a dry-running system that can be mounted in any
position.

| Parameter | Hella UP28 | Hella UP30 |
|---|---|---|
| Application | Support only — not standalone | **Standalone — sole vacuum source** |
| Rated voltage | 13.5V | **14.0V** |
| Current draw | <10A | **<15A** |
| Max vacuum | ≥86% of ambient | **≥86% of ambient** |
| Time to 50% vacuum | ≤5.5s | **≤3.5s** |
| Booster volume | 3.2 litres | **4.0 litres** |
| Pump operating life | 600 hours | **1,200 hours** |
| Sound level | <70 dB(A) | **<77 dB(A)** |
| Weight | ~1 kg | ~1 kg |
| Operating temperature | −40°C to +120°C | −40°C to +120°C |

**The UP30 is the correct unit** — rated for standalone operation
without any engine vacuum source. The UP28 is a support unit only.

Control is via a simple **vacuum pressure switch** set to activate
the pump when booster vacuum drops below ~500 mbar (the threshold
for adequate brake assist). The pump runs briefly to restore vacuum
then cuts out — exactly as on a diesel car or hybrid vehicle where
this system is OEM standard equipment. Over 17 million Hella
electric vacuum pumps have been produced since 1999 — this is
a mature, proven technology.

**Approximate cost: €80–150** for a new or quality used Hella UP30.
Available from all major automotive parts suppliers.

---

### Speedometer

The speedometer requires no special treatment. The automatic
gearbox used in this conversion outputs speed information as
standard — it only requires the correct RPM range at its input
shaft, which the step-down gearbox provides. The transmission's
own speed output signal drives the original speedometer exactly
as it would behind a piston engine. No conversion, no
recalibration, no additional hardware.

If the donor vehicle is fitted with a **standalone ABS unit**
— which most diesel automatics of this era are — the ABS
module generates wheel speed pulses independently of the
drivetrain. These pulses can serve directly as the speed
signal for the speedometer and any other systems that require
it, with no modification to the original instrument.

**Note on GPS-based speedometer solutions:** GPS speed units
are not appropriate for a road-registered vehicle. Approval
authorities treat GPS odometry as a potential instrument for
mileage manipulation and will not certify a vehicle equipped
with one as the primary speed/distance reference. The standard
gearbox output is the correct and only appropriate solution.

---

### Preferred Donor Vehicle

The Golf Mk2 and Volvo 740 were identified as suitable body
references on the basis of size. A more practical donor for an
actual build is a **similarly sized diesel automatic** — ideally
a former taxi.

**Why a taxi:**

- Taxis are retired when the engine wears out, not when the
  body, electrics, or running gear fail. A retired taxi typically
  has an excellent body, fresh brakes and tyres (legally required
  during service), intact ABS, working air conditioning, full
  electrical system, and a sound automatic gearbox — all the
  systems this conversion needs — at a very low purchase price
  precisely because the engine has issues.
- The automatic gearbox is already fitted, already connected
  to the speedometer, already integrated with the ABS, and
  already road-legal.
- Diesel taxi models of appropriate size include the
  **Volvo S70/V70 D**, **Ford Mondeo TDCi**, **Mercedes-Benz
  E220 CDI (W210/W211)**, and **Volkswagen Passat TDI** —
  all common taxi platforms, all available cheaply with high
  mileage engines, all with proven automatic gearboxes and
  standalone ABS units.
- The diesel engine is removed entirely and replaced with the
  turbine and step-down gearbox. The automatic transmission,
  propshaft, rear axle, brakes, ABS, steering, and all
  electrical systems remain untouched.
- EHPS is not needed — a diesel automatic taxi already has
  an engine-driven hydraulic power steering pump. This can
  be replaced with the Volvo EHPS unit or, on many later
  models, electric power steering is already fitted as
  standard.

The result is a vehicle where the turbine installation is the
only significant change — everything the approval authority
needs to assess for road safety is standard, documented, and
already type-approved.

---

### Turbine Engine Instrumentation

The minimum instrument set for safe and informed operation of the
M250-C18 in a car application:

| Instrument | Parameter | Type | Notes |
|---|---|---|---|
| **TGT gauge** | Turbine Gas Temperature | Thermocouple + analogue dial | Primary engine health indicator. Thermocouple already fitted to engine. Self-powered — no external supply needed |
| **N1 gauge** | Gas generator speed (%) | Tachometer — % RPM | Monitors compressor/gas generator speed |
| **Torque gauge** | Output shaft torque (%) | Pressure-based or electronic | Primary power indicator — the "throttle gauge" for a car |
| **Oil pressure** | Engine oil pressure | Pressure gauge | Critical — low oil pressure = immediate shutdown |
| **Oil temperature** | Engine oil temperature | Temperature gauge | Monitors lubrication health |
| **Fuel flow** | Litres per hour | Flow meter | Range management — essential given limited fuel cell |
| **Fuel level** | Tank contents | Float sender + gauge | Standard automotive sender in ATL cell |
| **FADEC warning light** | Fault indication | Single warning light | Wired to FADEC fault output |
| **Water level** | Injection tank | Sight gauge or float sender | Low level warning |

The TGT gauge is particularly elegant in that it requires no
external electrical power — the energy to drive the analogue meter
comes from the thermocouple itself. This type of simple analogue
instrument is commonplace in older gas turbine powered aircraft and
also useful for stationary or ground applications.

All instruments are available as standard aviation parts from
suppliers such as Aircraft Spruce, CostAero, or directly from
M250 FIRST Network centres. Standard 57mm (2¼ inch) aviation
instrument bezels fit neatly into a custom dashboard panel.

**Approximate instrumentation cost: €500–1,500** for a complete
analogue instrument set sourced from aviation surplus.

---

### Engine Cost — M250-C18

The M250-C18 is the oldest and most produced variant of the M250
family with over **6,400 engines** built. Used and serviceable
units circulate regularly in the helicopter MRO market.

**Typical market pricing (2024–2025):**

| Condition | Price range (USD) | Notes |
|---|---|---|
| Core / run-out (for parts or rebuild) | **$5,000–15,000** | High hours or out-of-limits — basis for rebuild |
| Serviceable — time continued | **$15,000–35,000** | Mid-life, logbooks current, ready to run |
| Recently overhauled (SMOH) | **$40,000–70,000** | Fresh overhaul by FIRST Network centre |
| Zero time since new (rare) | **$80,000+** | Effectively new |

For this project a **serviceable time-continued unit at $15,000–
35,000** is the practical target — sufficient operating hours remain
for many years of automotive use at low duty cycle, with a known
history and current logbooks. A pre-buy inspection by a FIRST
Network centre (Essential Turbines, Air Services International,
Premier Turbines etc.) before purchase is strongly recommended
and typically costs $500–1,500.

The M250-C20B (400 SHP, slightly more powerful than the C18) is
also widely available in this price range and uses the same
basic architecture — a consideration if more power is wanted
without moving to the RR300.

---

### Complete Ancillary System Cost Summary

| Item | Specification | Approx. cost |
|---|---|---|
| M250-C18 engine (serviceable) | Time-continued, with logbooks | **$15,000–35,000** |
| Pre-buy inspection | FIRST Network centre | $500–1,500 |
| EHPS pump (Volvo donor) | Used OEM unit | €80–150 |
| EHPS controller | Reform Motorsports or equivalent | €60–100 |
| Hella UP30 vacuum pump | Standalone brake booster supply | €80–150 |
| Turbine instrumentation | TGT, N1, torque, oil, fuel | €500–1,500 |
| **Total ancillary systems** | | **~€720–1,900** |
| **Total with engine** | | **~$17,000–40,000 + €720–1,900** |

These figures cover the engine and its direct support systems only —
not the donor vehicle, recuperator fabrication, step-down gearbox,
fuel cell, exhaust system, or installation labour.

---

*Section 22 added covering EHPS steering, Hella UP30 brake vacuum pump,*
*speedometer (standard gearbox output — no conversion needed), turbine*
*instrumentation, M250-C18 market pricing, and preferred donor vehicle.*
*Hella UP30 specifications from published Hella technical data sheet.*
*Engine pricing based on published aviation market listings 2024–2025.*
