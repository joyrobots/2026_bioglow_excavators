# FLL 2026 BIOGLOW Season: Innovation Project 12-Week Milestone Roadmap & FLL Rubrics Alignment Matrix

This roadmap aligns the Innovation Project with the five core criteria of the official FIRST LEGO League (FLL) Judging Rubrics: **Identify (3 Weeks)**, **Design (2 Weeks)**, **Create (3 Weeks)**, **Iterate (2 Weeks)**, and **Communicate (2 Weeks)** across five standardized engineering gates.

```text
┌─────────────────┐   ┌─────────────────┐   ┌─────────────────┐   ┌─────────────────┐   ┌─────────────────┐
│   Milestone 1   │──►│   Milestone 2   │──►│   Milestone 3   │──►│   Milestone 4   │──►│   Milestone 5   │
│    Identify     │   │     Design      │   │     Create      │   │     Iterate     │   │   Communicate   │
│    [3 Weeks]    │   │    [2 Weeks]    │   │    [3 Weeks]    │   │    [2 Weeks]    │   │    [2 Weeks]    │
└─────────────────┘   └─────────────────┘   └─────────────────┘   └─────────────────┘   └─────────────────┘
  Week 1 ~ Week 3       Week 4 ~ Week 5       Week 6 ~ Week 8       Week 9 ~ Week 10     Week 11 ~ Week 12

```

---

## Weekly Breakdown & Execution Plan

### 🟢 Milestone 1: Problem Identification & Research into Existing Solutions (Identify) — 3 Weeks

* **FLL Rubric Alignment:** **Identify** (Clear definition of a real-world problem, thorough multi-source research, comprehensive analysis of existing solutions and their limitations)


* **Timeline:** Week 1 – Week 3
* **Week 1: Ecological Orientation & Conceptual Exploration**
* **Instruction & Hands-on:** Explore core concepts of biodiversity and brainstorm how urban expansion and road construction fragment wildlife corridors (Habitat Fragmentation).


* **Deliverables:** Complete the "Local Wildlife Scouting Worksheet"; collect data on endangered and vulnerable species across the Greater Toronto Area (GTA) and York Region, and sketch initial protective mechanisms.




* **Week 2: Target Problem Formulation & Team Decision**
* **Instruction & Hands-on:** Each student presents their scouting findings; through team deliberation and consensus voting, officially select the **Jefferson Salamander crossing crisis on Stouffville Road in Richmond Hill** as the season's primary challenge; verify baseline biological data showing a **90% roadkill mortality rate** in the absence of wildlife corridors.


* **Deliverables:** Sign the team project charter; examine existing municipal mitigation infrastructure, including York Region's precast DECAST concrete box culverts ($3000\times1250\times2440\text{ mm}$) and plastic exclusion guide fences.




* **Week 3: Competitive Analysis & Expert Outreach Launch**
* **Instruction & Hands-on:** Benchmark against conventional ecological monitoring methods: highlight high stress from invasive fluorescent elastomer injections (VIE tagging), short 4–6 week battery lifespans of radio transmitters, and severe false triggers/optical blindness of traditional infrared trail cameras in rainy, murky conditions.


* **Deliverables:** Produce the "Defect Matrix of Existing Wildlife Monitoring Technologies"; finalize 3 high-value engineering inquiry questions focusing on "mid-transit turn-backs" and "adverse mud/water blind spots," and dispatch the expert inquiry email to the Toronto and Region Conservation Authority (TRCA) and York Region municipal environmental specialists.





---

### 🔵 Milestone 2: Innovative Solution & Real-World Feasibility (Design) — 2 Weeks

* **FLL Rubric Alignment:** **Design** (Originality/breakthrough nature of the solution, practical feasibility, clear consideration of engineering constraints and trade-offs)


* **Timeline:** Week 4 – Week 5
* **Week 4: Non-Invasive Architecture & Boundary Trade-offs**
* **Instruction & Hands-on:** Establish the core concept of a "100% Non-Invasive Automated Digital Audit Canopy"; address real-world municipal and ecological constraints (Trade-offs): municipal bans against structural drilling in concrete box culverts, raccoon tampering, and high-humidity short-circuiting.


* **Deliverables:** Formulate a non-destructive quick-mount protocol (industrial no-drill adhesive + 3M heavy-duty Dual Lock fasteners) and wiring protection specifications (ceiling-flush wire routing + 704 silicone sealant potting).




* **Week 5: Hardware Topology & Communication Protocols**
* **Instruction & Hands-on:** Overcome signal blockage inside underground concrete culverts (lack of 4G/cellular) and wet-environment cable degradation; design a hybrid network architecture using **ESP-NOW local wireless mesh for sub-millisecond timestamp sync + Bluetooth Low Energy (BLE) for drive-by zero-touch data harvesting**; finalize controller and sensor selection (M5Stack CoreS3 + ENV environmental probe + multi-channel vertical ToF laser distance sensors).


* **Deliverables:** Generate the "System Hardware & Communication Topology Map"; complete laser-cut CAD design files for the 1:5 transparent acrylic box culvert testing sandbox ($60\text{ cm}\times25\text{ cm}\times30\text{ cm}$).





---

### 🟡 Milestone 3: Working Functional Prototype & Physical Sandbox (Create) — 3 Weeks

* **FLL Rubric Alignment:** **Create** (Development of a working functional model/prototype that clearly demonstrates core operating principles and physical mechanics)


* **Timeline:** Week 6 – Week 8
* **Week 6: 1:5 Physical Sandbox Construction & Field Sampling (Field Trip 1)**
* **Instruction & Hands-on:** Assemble the transparent acrylic box culvert sandbox and lay out gravel substrates; conduct Field Trip 1 (scout the ecological corridor at 1071 Stouffville Rd, measure culvert geometry, test baseline wireless attenuation, and collect genuine site gravel samples).


* **Deliverables:** Complete full assembly of the 1:5 scale physical sandbox, surfacing the interior floor with genuine field gravel to replicate realistic optical reflections and sensor noise.




* **Week 7: Sensing Layer & Environmental Integration**
* **Instruction & Hands-on:** Mount the M5Stack CoreS3, ENV sensor, and multi-channel vertical ToF laser distance sensors to the sandbox ceiling; program environmental trigger thresholds (early spring nighttime rainfall + ambient temperature $>5^\circ\text{C}$ to wake the system from deep sleep).


* **Deliverables:** Display real-time ambient temperature and humidity telemetry on the CoreS3 screen with automated alert triggers.




* **Week 8: Directional Passage State Machine Validation**
* **Instruction & Hands-on:** Code the dual-beam sequential occlusion algorithm in UIFlow / MicroPython, determining animal transit status based on the millisecond timestamp delta between successive ToF triggers.


* **Deliverables:** Deliver an interactive working prototype: moving a salamander model through the sandbox triggers real-time status output on the screen distinguishing "Successful North-to-South Transit" from "Mid-Culvert Turn-Back".





---

### 🔴 Milestone 4: Robustness Testing & Engineering Iterations (Iterate) — 2 Weeks

* **FLL Rubric Alignment:** **Iterate** (Rigorous experimental testing, data-driven modifications based on failure points, evidence of multi-stage design evolution)


* **Timeline:** Week 9 – Week 10
* **Week 9: Substrate Noise Filtering & Architecture Reconstruction (V1 ➔ V2)**
* **Instruction & Hands-on:** Document the major architectural overhaul: transitioning from the early 40cm circular paper tube sandbox (V1) to the rectangular 3-track non-uniform laser canopy (V2), prompted by the discovery of DECAST's 2.8m internal clear width which caused massive blind spots with single-point sensors; engineer a moving average filter and an automated baseline surface scanning routine to eliminate false triggers from sharp gravel.


* **Deliverables:** Compile the "V1 to V2 Architecture Evolution Log"; plot the "False-Positive Rate Comparison Chart" demonstrating suppression of substrate-induced false triggers to below 2%.




* **Week 10: Environmental Stress Testing & Field Validation (Field Trip 2)**
* **Instruction & Hands-on:** Conduct Field Trip 2 (deploy the waterproofed engineering prototype at the Stouffville Rd culvert during rain to validate signal penetration and contactless BLE data harvesting); perform microclimate humidity and splash endurance testing; finalize the power consumption budget (verifying a 10,000 mAh battery pack sustains operations across the spring migration window).


* **Deliverables:** Document field logs with GPS coordinates and timestamps; seal and waterproof the modular field enclosures.





---

### 🟣 Milestone 5: Expert Feedback Loop & Presentation Pitch (Communicate) — 2 Weeks

* **FLL Rubric Alignment:** **Communicate & Core Values** (Sharing with diverse stakeholders, integrating professional expert critique, delivering an engaging, confident presentation with full team participation)


* **Timeline:** Week 11 – Week 12
* **Week 11: Integrating Expert Critique & Community Outreach**
* **Instruction & Hands-on:** Incorporate feedback received from TRCA and York Region municipal specialists into firmware updates (e.g., adding a warning flag for animal loitering/prolonged stay inside the culvert); demonstrate the 1:5 transparent sandbox system to teachers, peers, parents, and community conservation volunteers.


* **Deliverables:** Archive expert written correspondence and community evaluation forms; bind the 20–30 page "2026 BIOGLOW Innovation Project Engineering White Paper" (including CAD exploded-view diagrams, circuit schematics, and filtering algorithm snippets).




* **Week 12: 5-Minute Pitch Rehearsal & Defense Finalization**
* **Instruction & Hands-on:** Rehearse the 5-minute unscripted presentation utilizing the **"Because (harsh real-world constraints) ➔ But (conventional tech fails) ➔ So (engineered closed-loop solution)"** narrative framework; conduct high-pressure mock defense Q&A sessions covering budget, substrate false alarms, wireless shielding, and animal stress.


* **Deliverables:** Complete the tri-fold presentation showboard; lock in speaking roles across all team members and execute full-dress dry runs with live hardware demonstrations.





---

## 12-Week Roadmap vs. FLL Rubrics Gate Matrix

| Timeline | Milestone | FLL Official Rubric Criteria | Definition of Done (DoD) |
| --- | --- | --- | --- |
| **W1 ~ W3** | **M1: Identify**<br>

<br>(3 Weeks) | **Identify**<br>

<br>• Clear, well-defined problem statement<br>

<br>• Rigorous, multi-source evidence chain<br>

<br>• Thorough analysis of existing solutions and defects

 | • Identified Stouffville Rd Jefferson Salamander mortality (90% baseline)

<br>

<br>• Completed DECAST culvert engineering review & defect comparison matrix

<br>

<br>• Dispatched 3 technical inquiry questions to TRCA / York Region experts

 |
| **W4 ~ W5** | **M2: Design**<br>

<br>(2 Weeks) | **Design**<br>

<br>• Original, breakthrough concept<br>

<br>• Realistic, practical feasibility<br>

<br>• Articulated engineering constraints and trade-offs

 | • Finalized non-invasive overhead ToF laser canopy architecture

<br>

<br>• Resolved no-drill municipal restriction via no-drill mount specs

<br>

<br>• Designed ESP-NOW local sync & BLE data harvesting topology

 |
| **W6 ~ W8** | **M3: Create**<br>

<br>(3 Weeks) | **Create**<br>

<br>• Functional, working prototype<br>

<br>• Direct visual proof of core mechanisms<br>

<br>• Integrated hardware-software pipeline

 | • Assembled 1:5 scale acrylic sandbox using field-collected gravel

<br>

<br>• Deployed M5Stack CoreS3 with vertical ToF ranging arrays

<br>

<br>• Implemented real-time directional crossing and turn-back state machine

 |
| **W9 ~ W10** | **M4: Iterate**<br>

<br>(2 Weeks) | **Iterate**<br>

<br>• Rigorous experimental testing<br>

<br>• Design modifications driven by failure logs<br>

<br>• Multi-stage evolutionary iterations

 | • Documented V1 circular single-point to V2 3-track canopy redesign

<br>

<br>• Programmed adaptive ground baseline calibration (< 2% false alarm rate)

<br>

<br>• Executed rainy field deployment and environmental stress tests

 |
| **W11 ~ W12** | **M5: Communicate**<br>

<br>(2 Weeks) | **Communicate & Core Values**<br>

<br>• Direct collaboration with industry experts<br>

<br>• External critique incorporated into solution<br>

<br>• High-engagement, confident team presentation

 | • Received official expert written feedback and patched firmware

<br>

<br>• Bound 20–30 page engineering white paper and built pitch showboard

<br>

<br>• Polished 5-minute unscripted pitch with live prototype demo

 |
