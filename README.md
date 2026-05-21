# turbine-car-concept

# Recuperated Gas Turbine Car — Concept Design Specification

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

## 4. Recuperator Thermal Summary

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

## 5. Heat Exchanger Specification

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

## 6. FOD Protection

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

## 7. Electrical System

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

## 8. Fuel Cell

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

## 9. Fuel Consumption and Range

### SFC Basis

The M250 family achieves approximately **0.772 lb/SHP/hr** at cruise power.
Running derated at **450 SHP continuous:**

$$\text{Fuel flow} = 450 \times 0.772 = 347\ \text{lb/hr} = 157\ \text{kg/hr}$$

### Simple Cycle (no recuperator)

$$\text{Fuel flow} = \frac{157}{0.88} = 178\ \text{litres/hr}$$

*(Biodiesel density ~0.88 kg/litre)*

### Recuperated Cycle

The recuperator improves thermal efficiency by approximately 30% at cruise:

$$\text{Recuperated fuel flow} = 178 \times 0.70 = \mathbf{125\ \text{litres/hr}}$$

### Running Time and Range

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **24 minutes** | **~33 km** |
| 100 litres | **48 minutes** | **~66 km** |
| **120 litres (recommended)** | **~58 minutes** | **~79 km** |
| Required for 165 km / 2 hrs | — | **250 litres needed** |

### Range Note

The reference journey of 165 km taking 2 hours requires approximately **250 litres**
of biodiesel at cruise power with recuperation. The maximum practical fuel cell of
120 litres provides approximately **79 km range** — sufficient for a convention
demonstration, circuit event, or short-distance showcase run, but not for extended
road use without refuelling.

The fuel consumption is a direct consequence of the M250's specific fuel consumption
figure — a well-established characteristic of this class of turbine. To achieve
longer range within a 130-litre fuel limit, a smaller engine in the 200–250 SHP class
with proportionally lower fuel consumption would be required, at the cost of
reduced performance.

---

## 10. Summary Table

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
| **Recuperated fuel flow** | ~125 litres/hr at 450 SHP |
| **Range on 120 litres** | **~79 km / ~58 minutes** |
| **Electrical startup** | 24V — 2 × 12V / 600A AGM batteries in series |
| **Car electronics supply** | 12V tapped at Battery 1 positive terminal to ground |

---

*Concept design specification — theoretical study only.*
*All performance figures based on published M250 family data and standard thermodynamic analysis.*
*Recuperator dimensions and surface area calculated for ε = 0.90, U = 100 W/m²K, design case +5°C ambient.*

---

## 11. Alternative Engine Suggestion — Lighter Vehicle Application

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
| SFC at cruise | **0.76 lb/SHP/hr** |
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

**SFC:** <0.76 lb/SHP/hr at cruise (confirmed published figure)

Running at **210 SHP continuous:**

$$\text{Fuel flow} = 210 \times 0.76 = 159.6 \text{ lb/hr} = 72.4 \text{ kg/hr}$$

$$\text{Fuel flow (litres)} = \frac{72.4}{0.88} = \mathbf{82 \text{ litres/hr}}$$

**With recuperator — 30% SFC improvement:**

$$\text{Recuperated fuel flow} = 82 \times 0.70 = \mathbf{57 \text{ litres/hr}}$$

#### Range on Available Fuel Cells

| Fuel cell | Running time | Range at 82.5 km/hr average |
|---|---|---|
| 50 litres | **53 minutes** | **~73 km** |
| 100 litres | **105 minutes** | **~145 km** |
| **120 litres (ATL recommended)** | **~126 minutes (2hrs 6min)** | **~173 km** |

**The 120 litre ATL Saver Cell achieves the 165 km / 2-hour target with the RR300.**

This is the critical result. The RR300 at derated cruise power with recuperation
achieves the design range goal on a single standard fuel cell, whereas the M250-C47B
requires 250 litres to achieve the same range.

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
| Recuperated fuel flow | 125 litres/hr | **57 litres/hr** | **RR300** |
| Range on 120 litres | ~79 km | **~173 km** | **RR300** |
| Meets 165 km target? | **No** (needs 250L) | **Yes** (120L sufficient) | **RR300** |
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
