# Electrodynamics
電磁學
**Lecture Notes: The Wave Function**  
**Based on Sections 1.1–1.6**  

---

### **1.1 The Schrödinger Equation**  
**Key Concepts:**  
- **Classical vs. Quantum Mechanics**:  
  - *Classical*: Determines $ x(t) $ via Newton’s laws ($ F = ma $).  
  - *Quantum*: Seeks the wave function \( \Psi(x,t) \), governed by the **Schrödinger equation**:  
    $$
    i\hbar \frac{\partial \Psi}{\partial t} = -\frac{\hbar^2}{2m} \frac{\partial^2 \Psi}{\partial x^2} + V \Psi
    $$  
    Here, \( \hbar = h/2\pi \) (reduced Planck’s constant).  

- **Role of Initial Conditions**:  
  - Given \( \Psi(x,0) \), the Schrödinger equation predicts \( \Psi(x,t) \) for all \( t \), analogous to \( x(0) \) and \( v(0) \) in classical mechanics.  

---

### **1.2 The Statistical Interpretation**  
**Born’s Rule**:  
- \( |\Psi(x,t)|^2 \) is the **probability density** of finding the particle at \( x \).  
- Probability of locating the particle between \( a \) and \( b \):  
  \[
  \int_a^b |\Psi(x,t)|^2 dx
  \]  
- **Indeterminacy**: Quantum mechanics provides probabilities, not certainties.  

**Interpretations of Quantum Mechanics**:  
1. **Realist**: Particles have definite positions, but QM is incomplete (requires hidden variables).  
2. **Orthodox (Copenhagen)**: The particle has no definite position until measured.  
3. **Agnostic**: Rejects speculation about unmeasurable quantities.  

**Bell’s Theorem & Experiment**:  
- Experiments confirm the orthodox view: No hidden variables; measurement *creates* the outcome.  

**Wave Function Collapse**:  
- Measurement collapses \( \Psi(x,t) \) to a spike at the measured value (e.g., position \( C \)).  

---

### **1.3 Probability**  
#### **Discrete Variables**  
- **Probability**: \( P(j) = N(j)/N \).  
- **Expectation Value (Average)**:  
  \[
  \langle j \rangle = \sum j P(j)
  \]  
- **Variance & Standard Deviation**:  
  \[
  \sigma^2 = \langle j^2 \rangle - \langle j \rangle^2, \quad \sigma = \sqrt{\sigma^2}
  \]  

#### **Continuous Variables**  
- **Probability Density**: \( \rho(x) \), where \( \int_a^b \rho(x)dx = P_{ab} \).  
- **Normalization**: \( \int_{-\infty}^\infty \rho(x)dx = 1 \).  
- **Expectation Values**:  
  \[
  \langle x \rangle = \int x \rho(x)dx, \quad \langle f(x) \rangle = \int f(x)\rho(x)dx
  \]  

**Example 1.2 (Falling Rock)**:  
- Probability density for distance fallen: \( \rho(x) = \frac{1}{2\sqrt{hx}} \).  
- Average distance: \( \langle x \rangle = h/3 \).  

---

### **1.4 Normalization**  
**Requirement**:  
- \( \int_{-\infty}^\infty |\Psi(x,t)|^2 dx = 1 \).  
- Non-normalizable \( \Psi \) are unphysical.  

**Preservation of Normalization**:  
- Schrödinger equation ensures \( \frac{d}{dt} \int |\Psi|^2 dx = 0 \).  
- Proof uses integration by parts and boundary conditions (\( \Psi \to 0 \) as \( x \to \pm\infty \)).  

---

### **1.5 Momentum and Expectation Values**  
**Operators**:  
- Position: \( \hat{x} = x \).  
- Momentum: \( \hat{p} = -i\hbar \frac{\partial}{\partial x} \).  

**Expectation Values**:  
- \( \langle x \rangle = \int \Psi^* x \Psi dx \),  
  \( \langle p \rangle = \int \Psi^* \left(-i\hbar \frac{\partial}{\partial x}\right) \Psi dx \).  

**Ehrenfest’s Theorem**:  
- Expectation values obey classical equations:  
  \[
  \frac{d\langle p \rangle}{dt} = \left\langle -\frac{\partial V}{\partial x} \right\rangle
  \]  

---

### **1.6 The Uncertainty Principle**  
**Key Idea**:  
- Trade-off between precision in position (\( \sigma_x \)) and momentum (\( \sigma_p \)):  
  \[
  \sigma_x \sigma_p \geq \frac{\hbar}{2}
  \]  
- **Wave-Particle Duality**:  
  - Localized wave packet (\( \sigma_x \) small) → Broad momentum distribution (\( \sigma_p \) large).  
  - Extended wave (\( \sigma_x \) large) → Sharp momentum (\( \sigma_p \) small).  

**Example**:  
- Gaussian wave function minimizes \( \sigma_x \sigma_p \).  

---

### **Summary**  
1. **Wave Function** \( \Psi(x,t) \): Solution to Schrödinger equation; encodes probabilistic information.  
2. **Measurement**: Collapses \( \Psi \), introduces indeterminacy.  
3. **Operators**: Link observables (position, momentum) to mathematical operations.  
4. **Uncertainty Principle**: Fundamental limit on simultaneous knowledge of conjugate variables.  

---

**Further Topics**:  
- Problem 1.9: Gaussian wave packet and uncertainty.  
- Problem 1.18: Quantum vs. classical regimes (thermal de Broglie wavelength).  

**Conceptual Questions**:  
- How does the double-slit experiment illustrate wave-particle duality?  
- Why can’t the uncertainty principle be circumvented by better measurement technology?  

--- 

**Next Lecture**: Solutions to the Schrödinger equation in specific potentials.
