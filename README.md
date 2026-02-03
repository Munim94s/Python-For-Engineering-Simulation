# Python for Engineering Simulation (Not Data Science)

## Chapter 0 — How to Read This Book
- What this book is
- What this book is not
- Assumed background
- Why simulation is not reality
- How engineers misuse simulations

---

## Unit I — Foundations of Trustworthy Simulation

### Chapter 1 — What Simulations Are Allowed to Lie About
- Models vs reality
- Assumptions and abstractions
- Order-of-magnitude correctness
- When precision does not matter
- When it absolutely does

### Chapter 2 — Time Is the Enemy
- Continuous vs discrete time
- Fixed-step simulation philosophy
- Variable-step solvers and hidden dangers
- Aliasing, phase lag, and numerical damping
- Choosing a timestep like an engineer

---

## Unit II — Numerical Behavior (Without the Math Trauma)

### Chapter 3 — Numerical Stability Is Not Optional
- Euler integration and why it fails
- Runge–Kutta intuition
- Stiff systems explained physically
- Stability vs accuracy
- Why “it didn’t explode” is not success

### Chapter 4 — Energy, Conservation, and Silent Errors
- State variables and system energy
- Conservation laws as sanity checks
- Artificial damping and energy injection
- Detecting numerical drift

---

## Unit III — Modeling Real Physical Systems

### Chapter 5 — States, Inputs, and Outputs
- State-space thinking
- Separating physics from control
- Input saturation and limits
- Why unrealistic inputs ruin simulations

### Chapter 6 — Modeling Sensors and Actuators
- Ideal vs realistic sensors
- Noise, bias, and delay
- Actuator dynamics and lag
- Why perfect sensors break controllers

---

## Unit IV — Simulation for Control and Decision-Making

### Chapter 7 — Simulations Lie to Controllers
- Controller overfitting
- Gain sensitivity
- Stability margins vs simulated stability
- Why tuning in simulation fails in flight

### Chapter 8 — Validation, Verification, and Breaking Your Model
- Verification vs validation
- Known solutions and limiting cases
- Stress testing simulations
- Designing simulations to fail loudly

---

## Unit V — Practical Engineering Tradeoffs

### Chapter 9 — Performance, Real-Time, and Python’s Limits
- Timing guarantees
- The GIL and latency realities
- When Python is acceptable
- Hybrid Python/C architectures

### Chapter 10 — Case Study: A UAV That Looked Stable in Simulation
- System description
- Modeling assumptions
- What the simulation got wrong
- What failed in reality
- Lessons learned

---

## Appendix
- Common simulation anti-patterns
- Recommended libraries (and why)
- Further reading
- Notes on aerospace-grade simulation philosophy

---

## Closing Thoughts
- Simulation as a decision-support tool
- Engineering humility
- Why verification never ends

