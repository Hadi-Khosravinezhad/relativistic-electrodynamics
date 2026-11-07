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

---

## 📦 Step 2: The Moving Box & Matching Velocities 

To connect what the laboratory observer sees with what the internal observer experiences, we introduce a moving compartment (Frame $S'$).

### 1. The Key Condition: Synchronized Velocities
In the laboratory frame ($S$), consider two bodies moving together:
1. The **box** moving horizontally at velocity:  
   $$\mathbf{v}_{\text{box}} = v \hat{\mathbf{x}}$$
2. The **charged particle** placed inside the box, given the exact same initial horizontal velocity:  
   $$\mathbf{v}_{\text{particle}} = v \hat{\mathbf{x}}$$

### 2. Relative Velocity from Inside the Box (Frame $S'$)
Because the velocity of the particle strictly matches the velocity of the box, the relative velocity observed by the experimenter inside the box is identically zero:

$$\mathbf{v}'_{\text{particle}} = \mathbf{v}_{\text{particle}} - \mathbf{v}_{\text{box}} = v \hat{\mathbf{x}} - v \hat{\mathbf{x}} = \mathbf{0}$$

#### Physical Meaning:
- To the observer inside the box, the particle does not slide forward or backward.
- **The particle sits completely motionless right next to the observer.**
- Because uniform motion in an inertial frame cannot be sensed without external reference points, the observer perceives their entire compartment—and the particle resting inside it—as **completely at rest**.

---

### 3. The Sudden Dilemma: Why the Upward Motion Defies Magnetism
Now, the box carries this stationary particle into the region where an external magnetic field exists.

From the **Laboratory Frame ($S$)**:
* The particle has velocity $\mathbf{v} = v \hat{\mathbf{x}}$ in a field $\mathbf{B} = -B_0 \hat{\mathbf{z}}$.
* The magnetic force pulls it upward:  
  $$\mathbf{F} = q (\mathbf{v} \times \mathbf{B}) = +q v B_0 \hat{\mathbf{y}}$$
* The lab observer sees the particle rise naturally due to the magnetic force.

From the **Inside Frame ($S'$)**:
* The observer is watching a particle that was **strictly at rest** ($\mathbf{v}' = 0$).
* Suddenly, as the external field appears, the particle **spontaneously lifts off and accelerates straight upward!**
* The observer tests the magnetic hypothesis:
  $$\mathbf{F}'_{\text{mag}} = q (\mathbf{v}' \times \mathbf{B}') = q (\mathbf{0} \times \mathbf{B}') = 0$$
* Because the relative velocity is zero, **a magnetic field cannot exert a single Newton of force on this particle!**

### 💡 The Conclusion: The Inevitable Electric Field
If a stationary charge accelerates, the physical agent responsible must, by definition, be an **Electric Field ($\mathbf{E}'$)**:

$$\mathbf{F}' = q \mathbf{E}'$$

Since this force must balance the observed upward acceleration:

$$\mathbf{F}' = +q v B_0 \hat{\mathbf{y}}' \implies \mathbf{E}' = +v B_0 \hat{\mathbf{y}}'$$

> **The Grand Realization:**  
> The particle's horizontal motion was "hidden" from the internal observer.  
> Consequently, what the outside world measures as a **velocity-dependent magnetic force** ($\mathbf{v} \times \mathbf{B}$), the internal observer experiences directly as an **electrostatic-like field** ($\mathbf{E}'$).


https://github.com/user-attachments/assets/2efe91bd-7c4b-47c9-9a4e-0b2b1e757cd2

---

## ⚡ Step 3: The View from Inside the Box (The Emergence of the Electric Field)

Now, let us place ourselves entirely in the shoes of the observer inside the moving box (Frame $S'$). 

To this observer:
1. The walls of the box are completely motionless.
2. The particle is resting quietly on the floor ($x' = 0, y' = y_0$), with initial velocity:
   $$\mathbf{v}' = 0$$

Suddenly, as the box glides across the laboratory's field region, **the particle lifts off the floor and accelerates straight upward towards the ceiling!**

---

### 🔍 The Internal Observer's Deductive Reasoning

The observer inside wants to explain what physical force is causing this upward acceleration ($m \mathbf{a}'$):

1. **Could it be a Magnetic Force?**  
   The observer knows the magnetic Lorentz force formula:
   $$\mathbf{F}_{\text{mag}}' = q (\mathbf{v}' \times \mathbf{B}')$$
   However, the particle was initially **completely at rest** ($\mathbf{v}' = 0$).  
   A magnetic field cannot exert force on a stationary charge:
   $$\mathbf{v}' = 0 \implies \mathbf{F}_{\text{mag}}' = q (\mathbf{0} \times \mathbf{B}') = 0$$
   *Therefore, a magnetic field alone is mathematically incapable of initiating this motion!*

2. **The Only Possible Culprit: An Electric Field!**  
   In classical and modern electrodynamics, there is only **one** entity in the universe capable of accelerating a stationary charge from rest: an **Electric Field ($\mathbf{E}'$)**:
   $$\mathbf{F}' = q \mathbf{E}'$$

3. **Determining the Electric Field:**  
   Because the particle accelerates upward in the $+\hat{\mathbf{y}}'$ direction, the observer measures a net upward force:
   $$\mathbf{F}' = +q v B_0 \hat{\mathbf{y}}'$$
   Equating this to the electric force $q \mathbf{E}'$:
   $$q \mathbf{E}' = +q v B_0 \hat{\mathbf{y}}' \implies \mathbf{E}' = +v B_0 \hat{\mathbf{y}}'$$

---

### 🎬 Simulation: The Particle from Inside Frame $S'$

The animation below demonstrates the exact visual experience of the internal observer: the compartment is stationary, the particle sits at rest, and then accelerates vertically upward under the action of the induced electric field.

*(Add the uploaded video `box_inside_view.mp4` here using Drag & Drop)*

---

## 🎯 Final Synthesis: Resolving the Original Question

We now connect our physical thought experiment directly back to the original multiple-choice question:

> **Question:** In frame $S$, $\mathbf{B} = B_0 \hat{\mathbf{z}}$ and $\mathbf{E} = 0$. An observer in frame $S'$ moves with velocity $\mathbf{v} = v \hat{\mathbf{x}}$. To first order in $v/c$, what is $\mathbf{E}'$ observed in $S'$?

### 1. Vector Sign Relationship
In our simulation, we directed the magnetic field **into the screen** ($\mathbf{B} = -B_0 \hat{\mathbf{z}}$) to demonstrate an upward deflection ($+\hat{\mathbf{y}}$).

In the standardized test question:
* The magnetic field points **out of the screen**: $\mathbf{B} = +B_0 \hat{\mathbf{z}}$
* The relative frame velocity is to the right: $\mathbf{v} = v \hat{\mathbf{x}}$
* The force observed on a stationary charge in $S'$ is:
  $$\mathbf{F}' = q (\mathbf{v} \times \mathbf{B}) = q (v \hat{\mathbf{x}} \times B_0 \hat{\mathbf{z}}) = -q v B_0 \hat{\mathbf{y}}$$
* Therefore, the induced electric field is:
  $$\mathbf{E}' = -v B_0 \hat{\mathbf{y}} \quad \implies \mathbf{\text{Option (B) is strictly correct!}}$$

### 2. The Core Engineering Takeaway
For an electrical engineer:
* **Frame $S$ (Lab Frame):** Explains motional phenomena through $\mathbf{v} \times \mathbf{B}$ forces (e.g., Lorentz force on moving conduction electrons).
* **Frame $S'$ (Moving Frame):** Explains the exact same physical phenomena through an induced electric field $\mathbf{E}'$ (e.g., motional EMF: $\mathcal{E} = \int \mathbf{E}' \cdot d\mathbf{l}$).

**Electric and magnetic fields are not independent entities—they are two different manifestations of a single, unified electromagnetic field tensor, differing only by the state of motion of the observer.**



https://github.com/user-attachments/assets/dd98e731-110f-45dc-bfac-66a2edc85440

---










