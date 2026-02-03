# Python for Engineering Simulation (Not Data Science)

A practical guide to **engineering simulation using Python**, focusing on **physically meaningful and trustworthy results**. This repository accompanies the book content and provides guidance on **formatting, structure, and presentation** for technical readers.

---

## Content Overview

### Unit 0 — How to Read This Book
**Purpose:** Introduce the book’s philosophy and assumptions.

#### What this book is
- Practical guide for **engineering simulation** with Python  
- Focuses on **engineering thinking**: assumptions, checking results, understanding limitations  

#### What this book is not
- **Not a math textbook**: Avoids heavy derivations unless they aid intuition  
- **Not a data science/ML guide**: Focuses on **physical modeling**  
- **Not a Python tutorial**: Code illustrates concepts; production notes included only when necessary  

#### Prerequisites
- **Physics:** forces, energy, mechanics  
- **Calculus:** intuitive derivatives and integrals  
- **Python basics:** loops, functions, arrays  
- **Logical reasoning:** ability to detect unrealistic or breaking models  

#### Practical conventions
- **SI units**: consistent standard units  
- **Version control**: Git for tracking code iterations  
- **Python environment & libraries**: NumPy, SciPy, Matplotlib; optional JAX/Cython  
- **Code organization**: clean modules, commenting, and logging  

---

### Unit I — Foundations of Trustworthy Simulation
1. **Chapter 1 — What Simulations Are Allowed to Lie About**  
   - Models vs reality  
   - Assumptions and abstractions  
   - Order-of-magnitude correctness  
   - When precision does/does not matter  
   - **Why simulation is not reality**  
   - **How engineers misuse simulations**  

2. **Chapter 2 — Time Is the Enemy**  
   - Continuous vs discrete time  
   - Fixed-step simulation philosophy  
   - Variable-step solvers and hidden dangers  
   - Aliasing, phase lag, numerical damping  
   - Choosing a timestep like an engineer  

---

### Unit II — Numerical Behavior (Without the Math Trauma)
1. **Chapter 3 — Numerical Stability Is Not Optional**  
   - Euler integration and why it fails  
   - Runge–Kutta intuition  
   - Stiff systems explained physically  
   - Stability vs accuracy  
   - Why “it didn’t explode” is not success  

2. **Chapter 4 — Energy, Conservation, and Silent Errors**  
   - State variables and system energy  
   - Conservation laws as sanity checks  
   - Artificial damping and energy injection  
   - Detecting numerical drift  

---

### Unit III — Modeling Real Physical Systems
1. **Chapter 5 — States, Inputs, and Outputs**  
   - State-space thinking  
   - Separating physics from control  
   - Input saturation and limits  
   - Why unrealistic inputs ruin simulations  

2. **Chapter 6 — Modeling Sensors and Actuators**  
   - Ideal vs realistic sensors  
   - Noise, bias, and delay  
   - Actuator dynamics and lag  
   - Why perfect sensors break controllers  

---

### Unit IV — Simulation for Control and Decision-Making
1. **Chapter 7 — Simulations Lie to Controllers**  
   - Controller overfitting  
   - Gain sensitivity  
   - Stability margins vs simulated stability  
   - Why tuning in simulation fails in flight  

2. **Chapter 8 — Validation, Verification, and Breaking Your Model**  
   - Verification vs validation  
   - Known solutions and limiting cases  
   - Stress testing simulations  
   - Designing simulations to fail loudly  

---

### Unit V — Practical Engineering Tradeoffs
1. **Chapter 9 — Performance, Real-Time, and Python’s Limits**  
   - Timing guarantees  
   - The GIL and latency realities  
   - When Python is acceptable  
   - Hybrid Python/C architectures  

2. **Chapter 10 — Case Study: A UAV That Looked Stable in Simulation**  
   - System description  
   - Modeling assumptions  
   - What the simulation got wrong  
   - What failed in reality  
   - Lessons learned  

---

### Appendix
- Common simulation anti-patterns  
- Recommended libraries (and why)  
- Further reading  
- Notes on aerospace-grade simulation philosophy  

---

### Closing Thoughts
- Simulation as a decision-support tool  
- Engineering humility  
- Why verification never ends  

---

## Format and Style Guidelines

### Page Setup
- Page size: **6×9 inches** (or A4 for PDF/online)  
- Margins: 1 in top/bottom, 0.75–1 in left/right  
- Gutter (for print): 0.25–0.5 in

### Fonts
- Body: **Georgia**, 11–12 pt  
- Code: **Consolas**, 10–11 pt, monospace  
- Headings: **Arial or Open Sans**, bold

### Heading Hierarchy
| Level | Style | Example |
|-------|-------|---------|
| Unit | Heading 1, All Caps, 16–18 pt | UNIT I — FOUNDATIONS OF TRUSTWORTHY SIMULATION |
| Chapter | Heading 2, Bold, 14–16 pt | Chapter 1 — What Simulations Are Allowed to Lie About |
| Section | Heading 3, Bold, 12–14 pt | Models vs Reality |
| Subsection | Heading 4, Italic, 11–12 pt | Assumptions and Abstractions |

### Code Blocks
- Use **monospace font**, indentation preserved  
- Optional: gray background or table cell for emphasis  
- Line numbers optional  

### Figures and Tables
- Figures: centered, caption below (Figure 1.2)  
- Tables: caption above, numbered sequentially  

### Page Numbering
- Bottom-center or bottom-right  
- Optional header: chapter title  

### Additional Tips
- Line spacing: 1.15–1.2 for readability  
- Justify text for a professional look  
- Insert **page breaks** at chapter end (Ctrl + Enter)  
- Use Google Docs **heading styles** to auto-generate Table of Contents  

---

This README is intended to serve both as a **content map** and a **formatting guide**, making it easy to maintain consistency as the book grows.
