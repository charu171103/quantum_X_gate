# Quantum X Gate Demonstration

## Overview

The **Quantum X Gate** (also called the NOT gate or bit-flip gate) is one of the fundamental single-qubit gates in quantum computing. It flips the computational basis states:

- \( X|0\rangle = |1\rangle \)
- \( X|1\rangle = |0\rangle \)

Its matrix representation is:

\[
X = \begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
\]

This gate corresponds to a rotation by \(\pi\) radians (180°) about the X-axis on the Bloch sphere.

---

## Input States Considered

We demonstrate the effect of the X gate on four important quantum states:

1. \(|0\rangle = \begin{bmatrix}1 \\ 0\end{bmatrix}\)

2. \(|-\rangle = \frac{|0\rangle - |1\rangle}{\sqrt{2}} = \frac{1}{\sqrt{2}} \begin{bmatrix}1 \\ -1\end{bmatrix}\)

3. \(|i\rangle = \frac{|0\rangle + i|1\rangle}{\sqrt{2}} = \frac{1}{\sqrt{2}} \begin{bmatrix}1 \\ i\end{bmatrix}\)

4. \(|-i\rangle = \frac{|0\rangle - i|1\rangle}{\sqrt{2}} = \frac{1}{\sqrt{2}} \begin{bmatrix}1 \\ -i\end{bmatrix}\)

---

## Action of the X Gate on These States

### 1. On \(|0\rangle\):

\[
X|0\rangle = |1\rangle
\]

The X gate flips \(|0\rangle\) to \(|1\rangle\).

---

### 2. On \(|-\rangle\):

\[
X|-\rangle = -|-\rangle
\]

The X gate applies a **phase flip** (multiplies by \(-1\)) on the \(|-\rangle\) state.

---

### 3. On \(|i\rangle\):

\[
X|i\rangle = i |-i\rangle
\]

The X gate rotates \(|i\rangle\) into \(|-i\rangle\), introducing a phase factor of \(i\).

---

### 4. On \(|-i\rangle\):

\[
X|-i\rangle = -i |i\rangle
\]

Similarly, the X gate rotates \(|-i\rangle\) into \(|i\rangle\), with a phase factor of \(-i\).

---

## Summary Table

| Input State | Output State | Interpretation                  |
|-------------|--------------|--------------------------------|
| \(|0\rangle\) | \(|1\rangle\) | Bit flip                      |
| \(|-\rangle\) | \(-|-\rangle\) | Phase flip                    |
| \(|i\rangle\) | \(i|-i\rangle\) | Rotates to \(|-i\rangle\) with phase \(i\) |
| \(|-i\rangle\) | \(-i|i\rangle\) | Rotates to \(|i\rangle\) with phase \(-i\) |

---

## Intuition

- The X gate swaps the computational basis states \(|0\rangle\) and \(|1\rangle\).
- For superposition states \(|-\rangle\), \(|i\rangle\), and \(|-i\rangle\), it not only flips the basis components but can also introduce phase changes.
- This corresponds to a 180° rotation around the X-axis of the Bloch sphere, affecting both amplitude and phase of the qubit's state.

---

## Usage in the Notebook

This notebook demonstrates the matrix multiplication for each input state and visualizes the transformations on the Bloch sphere, helping you understand the geometric action of the X gate on various quantum states.

---

Feel free to explore and extend the notebook by adding simulations or other quantum gates!
