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

## 🧭 Step 1: The External Observer's Perspective: A Purely Magnetic Phenomenon

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

   $$\mathbf{F}'_{\text{mag}} = q (\mathbf{v}' \times \mathbf{B}')$$

   However, the particle was initially **completely at rest** ($\mathbf{v}' = 0$). A magnetic field cannot exert force on a stationary charge:

   $$\mathbf{v}' = 0 \implies \mathbf{F}'_{\text{mag}} = q (\mathbf{0} \times \mathbf{B}') = \mathbf{0}$$

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


https://github.com/user-attachments/assets/dd98e731-110f-45dc-bfac-66a2edc85440

---

## 🌀 Step 4: After Liftoff — The Awakening of the Magnetic Field (Frame $S'$)

In Step 3, we observed that the stationary charge was kicked into motion purely by the newly induced electric field:

$$\mathbf{E}' = +v B_0 \hat{\mathbf{y}}'$$

However, the story does not end with a simple upward acceleration. As soon as the particle acquires vertical velocity, a remarkable new physical effect emerges: **the magnetic field inside the moving box wakes up.**

---

### 1. The Magnetic Field Still Exists in Frame $S'$
According to the relativistic transformation of electromagnetic fields (at velocities $v \ll c$), the magnetic field measured in the moving frame remains virtually identical to that of the laboratory:

$$\mathbf{B}' \approx \mathbf{B} = -B_0 \hat{\mathbf{z}}'$$

Consequently, the interior of the moving box contains **both** an electric field and a magnetic field simultaneously:
* **Electric Field:** $\mathbf{E}' = +v B_0 \hat{\mathbf{y}}'$ (pulls upward)
* **Magnetic Field:** $\mathbf{B}' = -B_0 \hat{\mathbf{z}}'$ (acts on any moving charge)

---

### 2. The Emergence of the Backward Deflection
As the electric field accelerates the particle upward from rest, it acquires a vertical velocity component:

$$\mathbf{v}' = v'_y \hat{\mathbf{y}}' \quad (v'_y > 0)$$

Because the velocity is now non-zero, the magnetic Lorentz force equation inside the box is activated:

$$\mathbf{F}'_{\text{mag}} = q (\mathbf{v}' \times \mathbf{B}') = q \left( v'_y \hat{\mathbf{y}}' \times (-B_0 \hat{\mathbf{z}}') \right)$$

Applying the cross-product identity $\hat{\mathbf{y}}' \times \hat{\mathbf{z}}' = +\hat{\mathbf{x}}'$:

$$\mathbf{F}'_{\text{mag}} = -q v'_y B_0 \hat{\mathbf{x}}'$$

> 💡 **The Physical Revelation:**  
> The magnetic field does not push the particle upward; it pulls it **horizontally backward ($-\hat{\mathbf{x}}'$) toward the rear wall of the compartment!**

---

### 3. The Coupled Equations of Motion in Frame $S'$
At any subsequent time $t'$, the particle experiences the complete Lorentz force containing both fields:

$$\mathbf{F}' = \mathbf{F}'_{\text{elec}} + \mathbf{F}'_{\text{mag}} = q \mathbf{E}' + q (\mathbf{v}' \times \mathbf{B}')$$

Separating Newton's second law into Cartesian components:

$$\frac{dv'_x}{dt'} = -\frac{q B_0}{m} v'_y$$

$$\frac{dv'_y}{dt'} = \frac{q E'}{m} + \frac{q B_0}{m} v'_x = \frac{q v B_0}{m} + \frac{q B_0}{m} v'_x$$

Defining the cyclotron frequency $\omega = \frac{q B_0}{m}$ and the characteristic radius $R = \frac{v}{\omega} = \frac{m v}{q B_0}$:

$$\frac{d^2 x'}{dt'^2} = -\omega \frac{dy'}{dt'}$$

$$\frac{d^2 y'}{dt'^2} = \omega \left( v + \frac{dx'}{dt'} \right)$$

Integrating these coupled equations with initial conditions $\mathbf{r}'(0) = \mathbf{0}$ and $\mathbf{v}'(0) = \mathbf{0}$ yields the exact trajectory:

$$x'(t') = R \big( \sin(\omega t') - \omega t' \big)$$

$$y'(t') = R \big( 1 - \cos(\omega t') \big)$$

---

## 🎡 Step 5: The Cycloidal Trajectory & The Grand Invariance

The analytical solution above describes a **Cycloid** (the curve traced by a point on the rim of a rolling wheel).

<!-- PLACEHOLDER FOR CYCLOID PATH DIAGRAM / TRAJECTORY ANIMATION -->
https://github.com/user-attachments/assets/YOUR_CYCLOID_TRAJECTORY_ASSET_ID

### The Life Cycle of the Particle Inside the Box:
1. **Lift-off ($t'=0$):** The particle starts from rest at the floor; only $\mathbf{E}'$ acts, lifting it vertically upward ($+\hat{\mathbf{y}}'$).
2. **Backward Deflection ($0 < \omega t' < \pi$):** As vertical speed increases, $\mathbf{B}'$ pushes the particle backward ($-\hat{\mathbf{x}}'$).
3. **Crest ($\omega t' = \pi$):** The particle reaches maximum altitude ($y'_{\text{max}} = 2R$), where vertical velocity becomes zero and backward horizontal velocity peaks at $v'_x = -2v$.
4. **Descent & Cusp ($\pi < \omega t' < 2\pi$):** The backward motion reorients the magnetic force downward, returning the particle smoothly to the floor ($y'=0$), where it momentarily stops before repeating the cycle.

---

## 🎬 Numerical Simulation & Animation: The Dual-Field Cycloid

The animation below demonstrates the numerical simulation of the particle's full trajectory inside the moving compartment (Frame $S'$), showing the upward electric lift, backward magnetic deflection, and recurring cycloidal cusps:

<!-- PLACEHOLDER FOR SIMULATION VIDEO / GIF ASSET -->
https://github.com/user-attachments/assets/YOUR_SIMULATION_ANIMATION_ASSET_ID

---

## ⚖️ Reconciling the Two Frames: The Ultimate Test of Consistency

Do both observers agree on the physical outcome? **Yes, identically.**

| Feature | Laboratory Frame ($S$) | Moving Box Frame ($S'$) |
| :--- | :--- | :--- |
| **Observed Fields** | $\mathbf{E} = 0, \quad \mathbf{B} = -B_0 \hat{\mathbf{z}}$ | $\mathbf{E}' = v B_0 \hat{\mathbf{y}}', \quad \mathbf{B}' = -B_0 \hat{\mathbf{z}}'$ |
| **Active Force** | Purely Magnetic: $\mathbf{F} = q(\mathbf{v} \times \mathbf{B})$ | Dual: $\mathbf{F}' = q\mathbf{E}' + q(\mathbf{v}' \times \mathbf{B}')$ |
| **Trajectory Type** | Uniform Circular Motion | Cycloidal Motion |
| **Why does it lag backward?** | As the velocity vector turns upward, its horizontal velocity component drops ($v_x < v$). The box continues at constant speed $v$ and outpaces the particle. | The upward velocity through the magnetic field produces an active backward magnetic force: $\mathbf{F}' = -q v'_y B_0 \hat{\mathbf{x}}'$. |
| **Particle Coordinate** | $x(t) = R \sin(\omega t)$ | $x'(t') = x(t) - v t = R(\sin(\omega t') - \omega t')$ |
| **Vertical Coordinate** | $y(t) = R(1 - \cos(\omega t))$ | $y'(t') = y(t) = R(1 - \cos(\omega t'))$ |

---

## ⚡ Energy & Work: A Lesson in Relativity

* **In the Laboratory Frame ($S$):**  
  Because the magnetic force is perpendicular to velocity at every instant ($\mathbf{F} \perp \mathbf{v}$), the field does **strictly zero work** ($W = 0$). The particle's kinetic energy remains completely constant:

  $$K = \frac{1}{2} m v^2 = \text{const}$$

* **In the Moving Frame ($S'$):**  
  The electric field $\mathbf{E}'$ is parallel to the vertical displacement and **does real work** on the particle! The kinetic energy oscillates cyclically between $0$ (at the floor cusps) and $\frac{1}{2}m(2v)^2 = 2mv^2$ (at the peak of the cycloid).

> **Conclusion:**  
> Work and kinetic energy are not absolute constants—they depend fundamentally on the reference frame of the observer. What remains invariant is the physical reality described by the **Electromagnetic Field Tensor ($F^{\mu\nu}$)** across all inertial frames.
   









