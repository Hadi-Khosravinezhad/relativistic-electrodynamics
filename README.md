# Motional Electric Field in a Moving Reference Frame

A physical and numerical demonstration of motional electromagnetic fields, illustrating how a purely static magnetic field in one inertial frame induces an electric field from the viewpoint of a moving observer (to first order in $v/c$).

All computational implementations and visualizations are developed in Python / Jupyter Notebooks.

---

## 📌 Problem Statement

In an inertial reference frame $S$, there exists a uniform, static magnetic field with zero electric field:

$$\mathbf{B} = B_0 \hat{\mathbf{z}}, \quad \mathbf{E} = 0$$

An observer in reference frame $S'$ moves with non-relativistic velocity $\mathbf{v} = v \hat{\mathbf{x}}$ relative to frame $S$.

**Question:**  
To first order in $v/c$, what is the electric field $\mathbf{E}'$ observed in frame $S'$?

- (A) $\mathbf{E}' = v B_0 \hat{\mathbf{y}}$
- **(B) $\mathbf{E}' = -v B_0 \hat{\mathbf{y}}$**  *(Correct)*
- (C) $\mathbf{E}' = v B_0 \hat{\mathbf{z}}$
- (D) $\mathbf{E}' = 0$

---

## 💡 Physical Derivation: The Test-Charge Thought Experiment

Rather than relying on the formal machinery of Lorentz tensors or relativistic transformations, this result follows directly from classical mechanics and the consistency of physical forces across inertial frames in the non-relativistic limit ($v \ll c$).

### 1. The Laboratory Frame ($S$)
Consider a test charge $q$ that is held at rest inside the moving frame $S'$:
- To an observer in the lab frame $S$, this charge moves with a velocity:

  $$\mathbf{u} = \mathbf{v} = v \hat{\mathbf{x}}$$

- In frame $S$, the electric field is zero ($\mathbf{E} = 0$). The only force acting on the charge is the magnetic Lorentz force:

  $$\mathbf{F} = q (\mathbf{E} + \mathbf{u} \times \mathbf{B}) = q (0 + v \hat{\mathbf{x}} \times B_0 \hat{\mathbf{z}})$$

- Using the vector cross product ($\hat{\mathbf{x}} \times \hat{\mathbf{z}} = -\hat{\mathbf{y}}$):

  $$\mathbf{F} = -q v B_0 \hat{\mathbf{y}}$$

The observer in $S$ unambiguously observes the charge accelerating in the $-\hat{\mathbf{y}}$ direction.

### 2. The Moving Frame ($S'$)
Now examine the exact same physical event from the viewpoint of the moving observer in $S'$:
- In this frame, the charge is initially stationary ($\mathbf{u}' = 0$).
- Because the velocity is zero, the magnetic force on the charge in this frame is strictly zero:

  $$\mathbf{F}'_{\text{mag}} = q (\mathbf{u}' \times \mathbf{B}') = 0$$

- In Newtonian / non-relativistic physics ($v \ll c$), the net force acting on a body is frame-invariant:

  $$\mathbf{F}' = \mathbf{F}$$

- Since the charge is stationary in $S'$, the **only** physical entity that can exert a real force on it is an electric field $\mathbf{E}'$:

  $$\mathbf{F}' = q \mathbf{E}'$$

### 3. Equating the Forces
By equating the force observed in $S'$ to the force observed in $S$:

$$q \mathbf{E}' = \mathbf{F} = -q v B_0 \hat{\mathbf{y}}$$

Dividing by the charge $q$:

$$\mathbf{E}' = -v B_0 \hat{\mathbf{y}}$$

This confirms option **(B)** purely from force consistency and Galilean relativity.

---

## 🔬 Simulation Objectives

This repository provides numerical simulations to demonstrate:
1. **Force & Acceleration Equivalence:** Numerically integrating Newton's equation of motion $m \frac{d\mathbf{u}}{dt} = \mathbf{F}$ in both reference frames to confirm identical physical trajectories.
2. **Field Vector Visualizations:** Plotting the 2D vector field representation of the pure magnetic field in frame $S$ alongside the induced electric field $\mathbf{E}'$ in frame $S'$.

---

## 📂 Repository Structure

```text
motional-electric-field/
│
├── README.md                      # Problem formulation, physical derivation & documentation
├── requirements.txt               # Python package dependencies
│
├── notebooks/                     # Interactive Jupyter notebooks
│   └── simulation.ipynb
│
└── figures/                       # Generated high-resolution plots & diagrams (.png)
