# 01: Charged Particle Deflection (The External Observer's Perspective)

An analytical and computational investigation of a charged particle entering a static magnetic field, examined strictly from the laboratory reference frame ($S$).

---

## 📌 Problem Setup

Consider an external laboratory reference frame ($S$) with a defined spatial region containing a uniform, static magnetic field pointing perpendicularly into the page:

$$\mathbf{B} = -B_0 \hat{\mathbf{z}} \quad (\text{into the page } \otimes), \quad \mathbf{E} = 0$$

- For $x < 0$: The region is field-free ($\mathbf{B} = 0, \mathbf{E} = 0$).
- For $x \ge 0$: A uniform magnetic field $\mathbf{B} = -B_0 \hat{\mathbf{z}}$ is present.

A positive test charge ($q > 0$) travels from left to right along the horizontal axis with a constant initial velocity:

$$\mathbf{v} = v \hat{\mathbf{x}}$$

At $x = 0$, the particle crosses the boundary and enters the magnetic field region.

---

## 🧭 The External Observer's Perspective: A Purely Magnetic Phenomenon

To an external observer stationed at rest in the laboratory (frame $S$), this entire interaction is explained **strictly through classical magnetic forces**. No electric field exists in this frame, and none is needed to describe the physics.

### 1. Application of the Lorentz Force Law
The general Lorentz force equation acting on a charged particle is:

$$\mathbf{F} = q \left( \mathbf{E} + \mathbf{v} \times \mathbf{B} \right)$$

Because the external observer measures zero electric field ($\mathbf{E} = 0$), the force simplifies entirely to the magnetic component:

$$\mathbf{F} = \mathbf{F}_{\text{mag}} = q (\mathbf{v} \times \mathbf{B})$$

Substituting the velocity $\mathbf{v} = v \hat{\mathbf{x}}$ and magnetic field $\mathbf{B} = -B_0 \hat{\mathbf{z}}$:

$$\mathbf{F}_{\text{mag}} = q \left( v \hat{\mathbf{x}} \times (-B_0 \hat{\mathbf{z}}) \right) = -q v B_0 (\hat{\mathbf{x}} \times \hat{\mathbf{z}})$$

Using the vector cross-product identity $\hat{\mathbf{x}} \times \hat{\mathbf{z}} = -\hat{\mathbf{y}}$:

$$\mathbf{F}_{\text{mag}} = -q v B_0 (-\hat{\mathbf{y}}) = +q v B_0 \hat{\mathbf{y}}$$

### 2. Physical Conclusions in Frame $S$
- **Direction of Deflection:** The magnetic force acts continuously in the perpendicular $+\hat{\mathbf{y}}$ direction (upwards), pulling the particle into a smooth circular arc.
- **Zero Work Done:** Because $\mathbf{F}_{\text{mag}} \perp \mathbf{v}$ at all times:
  $$dW = \mathbf{F}_{\text{mag}} \cdot d\mathbf{r} = (\mathbf{F}_{\text{mag}} \cdot \mathbf{v}) dt = 0$$
  The magnetic field does strictly **zero work** on the particle. Its kinetic energy and speed ($|\mathbf{v}| = v$) remain constant, while only its direction of travel changes.
- **Verdict:** For the external observer, this is an open-and-shut case of magnetostatics—a moving charge deflected by a magnetic field.

---

## 🎬 Numerical Simulation & Animation

The numerical integration of Newton's equation of motion ($m \frac{d\mathbf{v}}{dt} = q \mathbf{v} \times \mathbf{B}$) illustrates this phenomenon clearly:



https://github.com/user-attachments/assets/32432c11-d852-474e-af70-518de70ce2ff

---

## 📦 Step 2: The Moving Box & The Principle of Relativity

To bridge the gap between classical electromagnetism and relativity, let us introduce a second observer into the experiment.

Imagine that our charged particle ($q$) is placed inside a closed, windowless compartment (a "box") that is moving horizontally to the right across the laboratory with constant velocity:

$$\mathbf{v}_{\text{box}} = v \hat{\mathbf{x}}$$

An experimenter (the **internal observer**, Frame $S'$) is stationed inside this box alongside the particle.

---

### 1. The Reality from the Outside (Laboratory Observer $S$)
To an engineer watching from the outside laboratory:
- Both the box and the charged particle are traveling at speed $v \hat{\mathbf{x}}$ through the uniform magnetic field $\mathbf{B} = -B_0 \hat{\mathbf{z}}$.
- The magnetic Lorentz force acts on the charge:
  $$\mathbf{F}_{\text{mag}} = q (\mathbf{v} \times \mathbf{B}) = +q v B_0 \hat{\mathbf{y}}$$
- Therefore, the external observer sees the particle **drift smoothly upward towards the ceiling of the box** as the box glides forward.
- Everything remains completely consistent with classical magnetostatics: the force is 100% magnetic.

---

### 2. The Experience from the Inside (Observer $S'$)
Now, consider the crucial question: **What does the observer inside the box feel and know?**

According to **Galileo’s Principle of Relativity** (and Einstein's First Postulate):
> *The laws of physics are identical in all inertial reference frames. Uniform rectilinear motion is physically undetectable from within a closed system.*

Because the box travels at a constant velocity without acceleration, shocks, or vibration:
1. **No Sensation of Motion:** The internal observer has **no physical way of knowing that the box is moving**. To them, the compartment feels completely stationary, just like sitting in a smooth high-speed train or an airplane cruising through still air.
2. **No Knowledge of the Outside World:** Because the box is sealed, the internal observer cannot measure their speed relative to the laboratory floor or look at the external magnets.
3. **The Puzzle:** From this observer's point of view, the box is their entire stationary universe. And yet, right before their eyes, **a stationary charged particle spontaneously lifts off and accelerates upward toward the ceiling!**

---

### 🎬 Simulation: The Moving Box from the Laboratory Frame

The animation below shows this scenario as observed by the external laboratory frame: the box glides across the magnetic field while the particle ascends within it.



https://github.com/user-attachments/assets/2efe91bd-7c4b-47c9-9a4e-0b2b1e757cd2

---








