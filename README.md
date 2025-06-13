# 🧠 Quantum X Gate Demonstration

This notebook demonstrates how the **Quantum X Gate** (also called the **quantum NOT gate**) acts on different quantum states.

---

## 🧮 What is the X Gate?

The **X gate** is a single-qubit quantum gate that flips the qubit state from `|0>` to `|1>` and vice versa. It's the quantum equivalent of the classical NOT gate.

### Matrix Representation:

```
X = [ 0  1 ]
    [ 1  0 ]
```

It swaps amplitudes of `|0>` and `|1>`:

```
X|0> = |1>
X|1> = |0>
```

---

## 🧬 Input States Tested

This notebook applies the X gate to the following states:

### 1. `|0>`

```
|0> = [1, 0]
X|0> = |1> = [0, 1]
```

---

### 2. `|-> = (|0> - |1>) / √2`

```
|-> = [1/√2, -1/√2]
X|-> = (|1> - |0>) / √2 = -|-> = [-1/√2, 1/√2]
```

🟢 **Note:** The global phase (like `-1`) has no physical meaning in quantum mechanics, so `- |->` is equivalent to `|->`.

---

### 3. `|i> = (|0> + i|1>) / √2`

```
|i> = [1/√2, i/√2]
X|i> = (|1> + i|0>) / √2 = [i/√2, 1/√2]
```

---

### 4. `|-i> = (|0> - i|1>) / √2`

```
|-i> = [1/√2, -i/√2]
X|-i> = (|1> - i|0>) / √2 = [-i/√2, 1/√2]
```

---

## 📊 Output and Observation

Each application of the X gate is shown with:

* The original state vector
* The matrix multiplication with the X gate
* The resulting state vector after transformation

These examples help in understanding how the X gate behaves not only on basis states but also on **superposition** and **complex phase** states.

---

## 📁 Contents of the Notebook

* `x_gate_matrix` – Numpy definition of the X gate
* State definitions for `|0>`, `|->`, `|i>`, and `|-i>`
* Application of the X gate using `numpy.dot()`
* Printed output for each case
* Optional visualization or explanation block (if added)

---

## 🧠 Why It Matters

Understanding how basic gates like **X** act on different quantum states builds your foundation for more complex operations in quantum circuits — like **quantum algorithms**, **error correction**, and **entanglement**.

---

## 🚀 Requirements

* Python 3.x
* Numpy
* Jupyter Notebook (optional, for interactive use)

Install with:

```bash
pip install numpy
```

