# MIT_Linear_Algebra_ARC_101

---

#### 🔰 Introduction: What Is Linear Algebra?

**Linear algebra** is a branch of mathematics that studies **vectors**, **vector spaces**, and **linear transformations** between these spaces. It's the foundation for solving **systems of linear equations**, modeling **real-world data**, and understanding **geometric transformations**. At its core, linear algebra answers questions like:

> "Can I find a unique solution that satisfies all these equations at once?"

---

# 🧩 What We Explored in This the MIT_LA_01

---

#### 1. **Solving 2 Equations with 2 Unknowns**

* We looked at a system like:

  $$
  \begin{aligned}
  3x + 2y &= 12 \\
  x - y &= 1
  \end{aligned}
  $$
* We plotted both **as lines** on a 2D graph and found their **intersection point**, which is the **solution** to the system.
* We learned: **2 independent linear equations in 2 variables** intersect at a **point** if a unique solution exists.

---

#### 2. **Visualizing Equations as Vectors**

* By treating each **column of the coefficient matrix** as a **vector**, we illustrated how the system `A·x = b` is a **linear combination of vectors**.
* Example:

  $$
  b = x \cdot v_1 + y \cdot v_2
  $$
* We plotted the **original vectors**, **scaled vectors**, and the **target vector** `b` to see how the solution builds from them.

---

#### 3. **Extending to 3 Equations and 3 Unknowns**

* We studied a 3×3 system:

  $$
  \begin{aligned}
  x + y + z &= 6 \\
  2x - y + z &= 3 \\
  x + 2y - z &= 4
  \end{aligned}
  $$
* Each equation forms a **plane** in 3D space.
* Their intersection point (if it exists) is the **unique solution** to the system.
* We visualized all 3 planes and confirmed they intersect at a single point.

---

#### 4. **Column Vectors in 3D**

* We interpreted the **columns of a 3×3 matrix** as **3D vectors**.
* By scaling and adding them based on the solution vector `[x, y, z]`, we reached the target vector `b`.
* This provided a **geometric understanding of matrix multiplication** as vector addition.

---

#### 5. **When Systems Cannot Be Solved**

We discussed what happens when there are:

* **Fewer equations than unknowns** (e.g., 8 equations in 9 variables):

  * The system is **underdetermined** → **infinite solutions** along a subspace.
* **Equations that are not linearly independent**:

  * The system cannot **fully constrain** the solution → **infinite or no solutions**.
* **Inconsistent equations**:

  * The planes or hyperplanes do **not intersect** at all → **no solution**.
___
# 🧩 What We Explored in This the MIT_LA_02

---

## 🧮 **Solving Systems of Linear Equations: Gaussian Elimination**

### ✅ **1. Gaussian Elimination (Concept)**

* Converts a system of linear equations $Ax = b$ into an **upper triangular form $Ux = y$**.
* Involves:

  * **Forward elimination**: Eliminate variables step-by-step from the lower rows.
  * **Backward substitution**: Solve for variables starting from the last equation.

### ✅ **2. Worked Example**

* We solved a 3×3 system of equations using forward elimination and backward substitution.
* Resulted in:

  $$
  x = 2.32,\quad y = 1.52,\quad z = 2.88
  $$

---

### ✅ **3. Procedural Code**

* Step-by-step Gaussian elimination in Python.
* Shows elimination and substitution stages clearly.

### ✅ **4. Matrix Form Using Elementary Matrices**

* Each row operation is represented by an **elementary matrix**.
* Gaussian elimination becomes:

  $$
  U = E_k \cdots E_2 E_1 A = EA
  $$
* Multiple row operations are combined into one matrix $E$.

---

## 🔁 **Permutation Matrices**

### ✅ **5. Row and Column Swapping**

* **Permutation matrices** are identity matrices with reordered rows or columns.
* Used to:

  * Swap rows: $P \cdot A$
  * Swap columns: $A \cdot P$
* Useful for **partial pivoting** to avoid division by zero or numerical instability.

---

## 🔢 **Why This Matters**

* Offers **deeper understanding** of Gaussian elimination as matrix operations.
* Foundation for **LU decomposition**, **numerical stability**, and **matrix factorization techniques**.
* Connects computational steps with **linear algebraic transformations**.

---

Let me know if you'd like all of this compiled into a PDF or notebook format—or to go deeper into LU, QR, or numerical issues like pivoting strategies!

