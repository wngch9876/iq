# Layer 1 — CCGT Plant Architecture

**Goal:** build a mental model of a combined cycle gas turbine plant detailed enough to interrogate a risk report and defend a PML.

**Output:** an annotated block diagram + equipment register for one reference plant.

---

## Step 1 — Reference plant (chosen)

**Mitsubishi Power M701JAC, 1×1 multi-shaft CCGT**

Headline specs (confirm against MHI brochure):
- Frequency: 50 Hz
- GT output (simple cycle): ~448 MW
- CCGT net output (1×1): ~650 MW
- Net CCGT efficiency: ~64%
- Turbine inlet temp class: 1650°C
- Cooling: air-cooled (the "AC" in JAC — distinguishes from steam-cooled earlier J-class)
- Typical fuel: natural gas (LNG common in Asia); some units dual-fuel with distillate

Why this config matters: in 1×1 multi-shaft, **GT and ST are on separate shafts with their own generators and GSUs**. GT can run simple-cycle if ST is unavailable — relevant for MBLOP scenarios.

---

## Step 2 — Equipment register (fill in)

For the chosen plant, list every major item with rating, OEM model, and one-line function.

### Gas turbine island
- Gas turbine (GT) — _model, MW, firing temp_
- GT auxiliaries — fuel gas system, lube oil, cooling air, IGV
- GT enclosure & fire protection

### Heat recovery steam generator (HRSG)
- HRSG — _make, pressure levels (HP/IP/LP), supplementary firing y/n_
- Stack, dampers, bypass (if any)

### Steam turbine island
- Steam turbine (ST) — _make, MW, HP/IP/LP sections_
- Condenser — _air-cooled vs water-cooled_
- Feedwater system, deaerator, BFP

### Electrical (note: 1×1 multi-shaft = 2 generators, 2 GSUs)
- GT generator — _MVA, cooling (air/H2/water), excitation_
- ST generator — _MVA, cooling, excitation_
- GT GSU transformer — _MVA, voltage ratio, OEM_
- ST GSU transformer — _MVA, voltage ratio, OEM_
- Switchgear, isolated phase bus per generator
- Station service / unit auxiliary transformer (UAT)

### Balance of plant (BoP)
- Cooling system — towers / ACC / once-through
- Water treatment, demin plant
- Fuel system — gas yard / liquid fuel backup
- Control system (DCS)
- Fire protection, civil structures

---

## Step 3 — Block diagram

Draw it (ASCII, drawio, or hand-sketched and photo'd). Goal: one page, every item from Step 2 visible, flows labelled (fuel, air, steam, water, electrical).

---

## Sources to read (pull from `references/`)

- IMIA WGP on Combined Cycle
- OEM technical brochure for chosen plant
- Gas Turbine World handbook entry for the model

---

## Next layer

Once this register exists → [Layer 2 — failure modes](layer2-failure-modes.md) hangs off each item above.
