# Birss: Conventions and Definitions Reference

**Source**: Compiled from full OCR extraction of scanned PDF pages 10–37 (printed book pages 1–55) of *Birss Symmetry & Magnetism komplett.pdf*, combined with transcribed Tables 3–4f and standard international crystallographic conventions. Sections 12–13 and the Table 6/7 cross-references additionally draw on Birss Chapter 3 (magnetic point groups, time-reversal/priming notation) via the transcribed `table-6.md`/`table-7.md`, not directly from the pages 10–37 OCR. Section 14 draws directly on Birss Chapter 2, §7 and Chapter 3, §5.

**Content Extracted**: 
- Scanned PDF pages 10–22 (printed pages 1–25): Introductory material, symbol definitions, single crystal structure
- Scanned PDF pages 23–37 (printed pages 26–55): Symmetry operations classification, generating matrices definitions, tensor form derivation procedures, and all 32 crystal classes reference diagram (Fig. 2.6)
- Chapter 3 (via Tables 6–7): Time-reversal (priming) notation for magnetic point groups, and the i-tensor/c-tensor symbol-class extension of Table 4a's scheme (§12, §13, and the "Extension to Magnetic Point Groups" part of §11)
- Chapter 2, §7 (printed pp. 71–73) and Chapter 3, §5 (printed pp. 122–124): "Null Property
  Tensors: 'Forbidden' Effects" — which tensor properties are identically zero in which
  (magnetic) crystal classes (§14)

---

## 1. Coordinate Axes and Orientation Conventions

### Crystal Coordinate System
- The crystal axes are denoted **Ox₁, Ox₂, Ox₃** (equivalently **x, y, z**, with $x_1=x$,
  $x_2=y$, $x_3=z$).
- These axes form a **right-handed orthonormal frame fixed in the crystal** (not
  necessarily the same as the crystallographic, possibly oblique, **a, b, c** axes — see
  the trigonal/hexagonal note below).
- **Per-system axis choice** (Birss Ch. 2, §1.4, and cross-checked against Table 4a's
  "Orientation of reference axes" column and the σ(N) table in §2):
  - **Triclinic**: no symmetry constraint on the axes.
  - **Monoclinic**: **z** is the **unique** symmetry axis — the 2-fold axis itself for
    class `2`, or the normal to the mirror plane for class `m` (Table 4a: `2//z`,
    `-2//z`). This is Birss's **z-unique** setting. It differs from the **b-unique**
    monoclinic convention common in International Tables for Crystallography — when
    comparing to such sources, `z` here plays the role that `b` plays there.
  - **Tetragonal, Trigonal, Hexagonal**: **z** is the principal axis (the 4-, 3-, or
    6-fold axis, = crystallographic `c`). **y** is either a secondary 2-fold axis
    perpendicular to z, for classes with `2⊥`/`-2⊥` operations such as `32`, `422`,
    `622` (matching generator σ(2) = [2_y], Table 4a: `2//y`), or the normal to a
    mirror plane containing z, for classes such as `3m`, `4mm`, `6mm` (matching
    generator σ(4) = [-2_y], Table 4a: `-2//y`). **x** completes the right-handed
    frame, perpendicular to both y and z. For trigonal/hexagonal crystals this
    orthonormal `x,y,z` frame is related to, but not identical to, the oblique
    crystallographic axes `c, a₁, a₂` (120° apart) — see Birss Fig. 1.1b / eq. (1.4)
    for that relation.
  - **Orthorhombic**: `x`, `y`, `z` are the three mutually perpendicular 2-fold axes
    (or mirror normals) — Table 4a: `2//x, 2//y` (the third, `2//z`, is implied).
  - **Cubic**: `x`, `y`, `z` lie along the cube edges — the three equivalent 4-fold or
    2-fold axes ([100]-type, Table 4a: `4//x, 4//y` or `2//x, 2//y`). The four 3-fold
    axes lie along the cube body diagonals ([111]-type) and are **not** coordinate
    axes (σ(9) realizes one such body-diagonal 3-fold by cyclically permuting x,y,z).

### Stereographic Projection Conventions
- The **principal symmetry axis** (highest-order rotation/rotation-inversion axis) is perpendicular to the projection plane and directed outward (normal to the page).
- The projection represents an **equatorial plane** of a reference sphere centered at the crystal origin.
- **Points above the plane** (emerging toward the observer) are marked with **●** (filled circle or dot).
- **Points below the plane** (receding away from the observer) are marked with **○** (empty circle).
- **Lines in the stereogram** represent poles to symmetry planes (great circles or their intersections).

---

## 2. Symmetry Operations and Classification

### Two Methods of Classification

**Method 1: Rotation and Rotation-Reflection Axes**
- **n-fold rotation axis**: Rotation by $2\pi/n$ around an axis.
- **n-fold rotation-reflection axis** (denoted $\bar{n}$ or S_n in Schoenflies): 
  - Rotation by $2\pi/n$ followed by reflection in a plane perpendicular to the rotation axis.
  - Example: For an object rotated then reflected, the sequence produces alternating congruent and reflected copies.

**Method 2: Rotation and Rotation-Inversion Axes** (Generally Preferred)
- **n-fold rotation axis**: Rotation by $2\pi/n$ around an axis (determinant +1).
- **n-fold rotation-inversion axis** (denoted $\bar{n}$ or improper rotation):
  - Rotation by $2\pi/n$ followed by **inversion through a fixed center point**.
  - Also called an **improper rotation** because it combines rotation with sense reversal.
  - Determinant: –1 for all improper rotations.
  - Example: $\bar{1}$ is pure inversion; $\bar{2}$ is equivalent to a mirror plane; $\bar{3}, \bar{4}, \bar{6}$ combine rotation with inversion.

### Identity Operation
- **E** (or **1**) = identity (no operation; rotation by 0°).
- **Determinant**: +1.
- Equivalent to a 1-fold rotation axis.

### Generating Matrices

Each crystal class has a **minimal set of generating matrices** σ(i), which when composed (multiplied) generate the entire point group.

**Key Properties:**
- All are **3×3 orthogonal matrices** acting on coordinates: $\vec{x}' = \mathbf{g} \vec{x}$.
- $\mathbf{g}^T \mathbf{g} = \mathbf{I}$ (orthogonality).
- $\det(\mathbf{g}) = +1$ for proper rotations; $-1$ for improper rotations.

### The σ(0)–σ(9) Matrix Pool

Birss equation (2.17) (scanned PDF page 34, printed page 48) defines a fixed pool of ten named
3×3 matrices, σ(0)–σ(9). Table 3's "Generating matrices" column and Table 6's
σ(N)/σ'(N) columns reference these by number. The axis labels in the "Operation"
column below (`2_y`, `4_z`, etc.) are the same axis labels used in Table 3's "Symmetry
operations" column — e.g. Table 3's class `2` lists operation `2_z` and generator
σ(3), and indeed σ(3) = [2_z] below.

| σ(N) | Symbol | Matrix | Operation |
|---|---|---|---|
| σ(0) | [1] | $\begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}$ | Identity |
| σ(1) | [-1] | $\begin{pmatrix}-1&0&0\\0&-1&0\\0&0&-1\end{pmatrix}$ | Inversion |
| σ(2) | [2_y] | $\begin{pmatrix}-1&0&0\\0&1&0\\0&0&-1\end{pmatrix}$ | 2-fold rotation about y |
| σ(3) | [2_z] | $\begin{pmatrix}-1&0&0\\0&-1&0\\0&0&1\end{pmatrix}$ | 2-fold rotation about z |
| σ(4) | [-2_y] | $\begin{pmatrix}1&0&0\\0&-1&0\\0&0&1\end{pmatrix}$ | Mirror ⊥ y (= –2_y) |
| σ(5) | [-2_z] | $\begin{pmatrix}1&0&0\\0&1&0\\0&0&-1\end{pmatrix}$ | Mirror ⊥ z (= –2_z) |
| σ(6) | [3_z] | $\begin{pmatrix}-\frac{1}{2}&\frac{1}{2}\sqrt{3}&0\\-\frac{1}{2}\sqrt{3}&-\frac{1}{2}&0\\0&0&1\end{pmatrix}$ | 3-fold rotation (120°) about z |
| σ(7) | [4_z] | $\begin{pmatrix}0&1&0\\-1&0&0\\0&0&1\end{pmatrix}$ | 4-fold rotation about z |
| σ(8) | [-4_z] | $\begin{pmatrix}0&-1&0\\1&0&0\\0&0&-1\end{pmatrix}$ | –4 roto-inversion about z |
| σ(9) | (cyclic) | $\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}$ | 3-fold rotation about the [111] body diagonal (cyclic permutation x→y→z→x) |

Primed matrices σ'(N) denote the same matrix σ(N) combined with time reversal (see §12).

**Example:** For class **32** (D₃, trigonal), Table 3 lists generators **σ(2), σ(6)**:
- σ(2) = [2_y]: a 2-fold axis perpendicular to the principal axis (Table 3's `3(2⊥)` operations)
- σ(6) = [3_z]: the 3-fold principal axis (the `±3_z` operations)

Composing these two generates all 6 symmetry operations of the group (1, two `±3_z`
rotations, and three `2⊥` axes).

**Example:** For class **6/mmm** (D₆h, hexagonal, highest symmetry), Table 3 lists
**four** generators — σ(1), σ(2), σ(3), σ(6) — this is the book's own worked example,
equation (2.19):
- σ(1) = [-1] (inversion)
- σ(2) = [2_y]
- σ(3) = [2_z]
- σ(6) = [3_z]

Composing these generates all 24 symmetry operations of 6/mmm. See §5 for how this
generator set is used to derive a tensor's reduced form.

**Relation to Point Group Symbols:** The generating matrices provide the actual mathematical implementation of the symmetry operations denoted by Hermann–Mauguin and Schoenflies symbols.

---

## 3. Point Group Nomenclature

### International (Hermann–Mauguin) Notation
Describes the **symmetry elements** of the point group using a standardized convention:

- **n** = n-fold rotation axis (1, 2, 3, 4, 6)
- **–n** or **n̄** = n-fold roto-inversion axis (barred or with overline)
- **m** = mirror plane (reflection plane)
- **·** or **/** = separator indicating **perpendicular or independent** symmetry directions
  - Example: `2/m` means a 2-fold axis with a mirror plane perpendicular to it
  - Example: `m.2.m` means a mirror plane, perpendicular 2-fold axis, and another mirror plane
  - In Shubnikov notation, typically represented as a **dot** (e.g., `2.m`)

**Abbreviated vs. Full Notation:**
- Abbreviated form omits redundant generators (e.g., `mmm` instead of `m.m.m`)
- Full form explicitly lists all principal symmetry elements

### Schoenflies Notation
Point group classification using symbols with subscripts (now displayed with HTML `<sub>` tags):

- **C_n** = Cyclic group with n-fold axis (rotation only)
- **C_{nh}** = Cyclic group with n-fold axis **and** horizontal mirror plane (perpendicular to principal axis)
- **C_{nv}** = Cyclic group with n-fold axis **and** vertical mirror planes (containing principal axis)
- **S_n** = Improper (roto-inversion) axis of order n (no proper n-fold axis)
- **D_n** = Dihedral group with n-fold axis and n perpendicular 2-fold axes
- **D_{nh}** = Dihedral group with horizontal mirror plane
- **D_{nd}** = Dihedral group with diagonal (vertical) mirror planes
- **T, T_h, T_d** = Tetrahedral groups (cubic with 3-fold axes along [111] directions)
- **O, O_h** = Octahedral groups (cubic with highest symmetry)

### Shubnikov Notation
Notation emphasizing the presence of inversion symmetry; uses **dots**, **colons**, and
(for cubic classes) **slashes** as separators:

- **n.m** means n-fold axis with m mirror planes (containing/parallel to the axis)
- **–n** (barred) prefix indicates inversion-related elements
- Example: `2.m` = 2-fold axis with a parallel mirror plane (International class mm2)
- Example: `–6.m` = –6 roto-inversion axis with mirrors (International class –3m, Table 3)
- **`:`** separates a principal rotation axis from a **perpendicular** set of secondary
  axes or mirrors, e.g. `2:m` (class 2/m: 2-fold axis, mirror ⊥ to it), `2:2` (class 222),
  `4:m`, `6:m`. A leading `m.` combined with a `:` group, e.g. `m.2:m` (class mmm) or
  `m.6:m` (class 6/mmm), reads as "mirror, plus axis-with-perpendicular-mirror".
- **`/`** is used only for the **cubic** classes, separating the symbol for the
  body-diagonal ([111]-type) 3-fold/–6 axes from the symbol for the coordinate-axis
  ([100]-type) 2-fold/4-fold axes, e.g. `3/2` (class 23), `3/4` (class 432), `–6/4`
  (class m3m). See Table 3's "Shubnikov" column for the full set of 32 symbols.

---

## 4. Symmetry Operation Symbols

### Proper Rotation Axes
| Symbol | Name | Order | Rotation Angle | Determinant |
|---|---|---|---|---|
| 1 or **E** | Identity | 1 | 0° | +1 |
| 2 | 2-fold (dyad) | 2 | 180° | +1 |
| 3 | 3-fold (triad) | 3 | 120° | +1 |
| 4 | 4-fold (tetrad) | 4 | 90° | +1 |
| 6 | 6-fold (hexad) | 6 | 60° | +1 |

### Improper Rotation (Roto-Inversion) Axes
| Symbol | Name | Operation | Determinant | Note |
|---|---|---|---|---|
| **-1** | Inversion center | Inversion through point | -1 | Pure inversion; identity rotation + inversion |
| **-2** | Mirror plane | 180° rotation + inversion = reflection | -1 | Equivalent to m; perpendicular to axis |
| **-3** | 3-fold roto-inversion | 120° rotation + inversion | -1 | Distinct improper operation |
| **-4** | 4-fold roto-inversion | 90° rotation + inversion | -1 | Distinct improper operation |
| **-6** | 6-fold roto-inversion | 60° rotation + inversion | -1 | Distinct improper operation |

### Mirror Planes and Perpendicular Axes
- **m** = Mirror plane (reflection); equivalent to **-2** (see table above).
- In the **symmetry operations** column of Tables 3, 4c–4f, and 6, notation like:
  - `2_z` = 2-fold axis along z-direction.
  - `-2_z` = Mirror plane perpendicular to z (equivalent to roto-inversion).
  - `2⊥` = 2-fold axis **perpendicular** to the principal axis (replacing the book's perpendicular symbol).
  - `-2⊥` = Mirrors perpendicular to the principal axis.

### Plus/Minus Notation
- **±** is the preferred symbol for "plus or minus" pairs of symmetry operations (e.g. `±3_z`, `±4_z`,
  `±6_z`, `4(±3)`). The book's `+/-` notation should be written as `±` consistently across all tables.

### Multi-Fold Operations
- **n(m)** in symmetry operations (e.g., `3(2⊥)`) denotes **n equivalent m-fold axes**.
  - Example: `3(2⊥)` = three 2-fold axes perpendicular to the principal 3-fold axis.
  - Example: `3(-2⊥)` = three mirror planes perpendicular to the principal 3-fold axis (e.g., in class 3m).
  - Example: `6(2⊥)` = six 2-fold axes perpendicular to a principal 6-fold axis.
  - Example: `6(-2⊥)` = six mirror planes perpendicular to a principal 6-fold axis (e.g., in class 6mm).

- **n(k)** or **n(m₁), n(m₂)** groups together **n equivalent symmetry elements**.

### Cyclic Permutations and Restricted Permutations
- **xxyz(c4)** = Four **cyclic permutations** of indices: `xxyz, yzxx, zxxy, xyzx`. (Used in rank-4 tensors.)
- **zzxy(xy:6)** = Six permutations of `zzxy` **preserving the order x, y**:  
  `zzxy, zzyx, zyxx, zyxy, zxyy, zxyy` (variations with x, y in fixed relative order).

---

## 5. Deriving Tensor Forms: Systematic Procedure

### General Method (§5 of Birss Chapter 2)

To find the independent components of a property tensor of rank **m** in a specific crystal class:

1. **Choose the generating matrices** σ(i) for that class (from Table 3, column 8).

2. **Apply the constraint equation** for polar tensors:
   $$\mathbf{d}_{ij...k} = \sum_n O_{i p} O_{j q} \cdots O_{k r} d_{pq...r}$$
   where the $O_{ij}$ are components of each generating matrix $\sigma$.

3. **For axial tensors**, apply the same equation with an additional factor of $\det(\sigma)$:
   $$\mathbf{d}_{ij...k} = \det(\sigma) \sum_n O_{i p} O_{j q} \cdots O_{k r} d_{pq...r}$$

4. **Systematically substitute** each generating matrix into the constraint equation.

5. **Collect all independent coefficients** that satisfy all constraints simultaneously.

### Example: Fourth-Rank Tensor in Class 6/mmm

For the hexagonal class **6/mmm**, Table 3 lists four generating matrices — σ(1), σ(2), σ(3), σ(6) (Birss equation 2.19):

$$\sigma(1) = \begin{pmatrix} -1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & -1 \end{pmatrix}, \quad \sigma(2) = \begin{pmatrix} -1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & -1 \end{pmatrix}, \quad \sigma(3) = \begin{pmatrix} -1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{pmatrix}, \quad \sigma(6) = \begin{pmatrix} -\frac{1}{2} & \frac{1}{2}\sqrt{3} & 0 \\ -\frac{1}{2}\sqrt{3} & -\frac{1}{2} & 0 \\ 0 & 0 & 1 \end{pmatrix}$$

Since σ(1) is an inversion (determinant = –1), all **axial** fourth-rank tensors vanish identically in this class. For **polar** tensors, applying each matrix to the general rank-4 tensor produces sets of constraints (detailed in Birss equations 2.20–2.22).

The result is that the independent components reduce to a minimal set, determined by which coefficients remain after all constraints are applied.

### Worked Example: Polar Rank-2 Tensor in Class 2/m

This example carries the procedure all the way through to a Table 4d row, for a
smaller (rank-2) case. Table 3 lists class **2/m** (C₂h) with generators **σ(1), σ(3)**:

$$\sigma(1) = \begin{pmatrix} -1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & -1 \end{pmatrix}, \qquad \sigma(3) = \begin{pmatrix} -1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$$

A general polar rank-2 tensor has 9 components $d_{ij}$ ($i,j \in \{x,y,z\}$). Apply
the constraint $d_{ij} = O_{ip}O_{jq}d_{pq}$ for each generator:

**Step 1 — σ(1) (inversion):** $O_{ip} = -\delta_{ip}$, so
$O_{ip}O_{jq}d_{pq} = (-\delta_{ip})(-\delta_{jq})d_{pq} = d_{ij}$. The constraint
$d_{ij} = d_{ij}$ is trivially true for every component — inversion imposes **no**
restriction on a polar rank-2 (even-rank) tensor, as expected from the rule above.

**Step 2 — σ(3) ($2_z$):** $O = \mathrm{diag}(-1,-1,1)$ is diagonal, so
$O_{ip}O_{jq}d_{pq} = O_{ii}O_{jj}d_{ij}$ (no sum). The sign factor $O_{ii}O_{jj}$ is
$+1$ if $i,j$ are both in $\{x,y\}$ or both equal to $z$, and $-1$ if exactly one of
$i,j$ is $z$:

| Component | $O_{ii}O_{jj}$ | Constraint | Result |
|---|---|---|---|
| $d_{xx}, d_{yy}, d_{zz}$ | $+1$ | $d_{ii}=d_{ii}$ | survives |
| $d_{xy}, d_{yx}$ | $(-1)(-1)=+1$ | $d_{xy}=d_{xy}$ | survives |
| $d_{xz}, d_{zx}, d_{yz}, d_{zy}$ | $(-1)(1)=-1$ | $d_{iz}=-d_{iz}$ | $=0$ |

**Step 3 — Reduced form:** the independent, non-vanishing components are
$d_{xx}, d_{yy}, d_{zz}, d_{xy}, d_{yx}$; all components with exactly one $z$ index
vanish.

**Step 4 — Confirm via Table 4a/4d:** Table 4a gives class `2/m` the symbol class
`B_m` for "Polar tensor of even rank m" (with reference axes `2//z`, matching σ(3)'s
axis). At $m=2$, row **B2** of Table 4d reads `xx | yy | zz | xy | yx | 0 | 0` for
columns `xx, yy, zz, xy, yx, xz(2), yz(2)` — exactly the reduced form derived above.

### Tensor Equalities Between Crystal Classes

**Key Principle**: Different crystal classes may yield identical tensor forms for the same rank.

- In class **2** (C₂): relation $\sigma = -\sigma(2)$ (for example)
- In class **m** (C_s): relation $\sigma = \sigma(1)$ (mirror plane)
- In class **2/m** (C₂h): σ(1) and σ(3) are generating matrices

**Consequence**: Polar tensors of even rank are equal in class **2** and **m**; axial tensors of odd rank are equal in these classes.

For **centrosymmetrical** classes (containing inversion, σ(1)):
- Polar tensors of **odd** rank vanish entirely; polar tensors of **even** rank survive
  (the two factors of $-1$ from $O_{ip}O_{jq}$, applied an even number of times, cancel).
- Axial tensors of **even** rank vanish entirely; axial tensors of **odd** rank survive
  (the extra $\det(\sigma)=-1$ factor flips the parity relative to the polar case).

(Confirmed against Table 4a: class `2/m` has `-` for both "Axial tensor of even rank"
and "Polar tensor of odd rank", but `B_m`/`B_n` for "Polar tensor of even rank"/"Axial
tensor of odd rank".)

**Table 4a Reference**: Lists which tensor symbols ($B_n$, $B_m$, etc.) represent identical forms across different crystal classes. The same symbol appearing in multiple rows indicates equivalent tensors.

### Practical Lookup: Tables 4b–4f

Rather than deriving tensors from scratch, the independent components for each rank in each crystal class are tabulated:

- **Table 4b** (rank 0): Scalars — single component in all classes
- **Table 4c** (rank 1): Vectors — components x, y, z with zeros showing which vanish
- **Table 4d** (rank 2): Symmetric rank-2 tensors — 7 component groups
- **Table 4e** (rank 3): Rank-3 tensors — 15 component groups
- **Table 4f** (rank 4): Rank-4 tensors — up to 25 component groups

Each **row** represents a crystal class; each **column** shows the reduced form of that component in that class (0 = vanishes, variable symbol = survives and is independent).

## 6. Tensor Component Notation (Tables 4b–4f)

### Grouped Component Notation
The tables use **subscript counts** in parentheses to denote **equivalent components under the group**:

| Notation | Meaning | Example Count |
|---|---|---|
| `xx, yy, zz` | Single components (no grouping) | 1 each |
| `xy(2)` | Two equivalent unrestricted permutations | `xy, yx` |
| `xxy(3)` | Three unrestricted permutations | `xxy, xyy, yxx` |
| `xxxz(4)` | Four unrestricted permutations | `xxxz, yxxz, zxxx, xxyy` (etc.) |
| `yxxx(x·3)` | Three components by **fixing last index** and permuting others | `yxxx, xxyy, xxxx` |
| `xxyy(x:3)` | Three components by **fixing first index** and permuting others | `xxyy, xzyz, xyyz` |
| `xxyz(c4)` | Four **cyclic permutations** | `xxyz, yzxx, zxxy, xyzx` |
| `zzxy(xy:6)` | Six permutations **preserving x, y order** | `zzxy, zzyx, ...` (6 distinct) |

### Minus Signs in Tables
- **Minus signs** (e.g., `-xx`, `-xy`, `-2_z`) denote **barred symmetry elements** or **inversion-related** components.
- **0** indicates that component **vanishes** in that crystal class.

---

## 7. Crystal Classes Reference (32 Point Groups)

All 32 crystallographic point groups are organized in **Fig. 2.6** (scanned PDF page 30, printed pages 40–41) by crystal system:

- **Triclinic**: 1, –1
- **Monoclinic**: 2, m, 2/m
- **Orthorhombic**: 222, mm2, mmm
- **Tetragonal**: 4, –4, 4/m, 422, 4mm, –42m, 4/mmm
- **Trigonal**: 3, –3, 32, 3m, –3m
- **Hexagonal**: 6, –6, 6/m, 622, 6mm, –6m2, 6/mmm
- **Cubic**: 23, m3, 432, –43m, m3m

Each class has:
- Generating matrices in **Table 3, column 8**
- Tensor forms for each rank in **Tables 4b–4f**

**Centrosymmetrical Classes** (containing inversion center –1):
- –1, 2/m, mmm, 4/mmm, –3m, 6/mmm, m3, m3m
- In these classes, polar tensors of odd rank vanish and axial tensors of even rank
  vanish (see §5, "Tensor Equalities Between Crystal Classes")

---

## 8. Key Findings from Pages 23–37 (printed pages 26–55)

### Symmetry Operation Enumeration

For any point group, symmetry operations can be enumerated using:

1. **Rotation axes** (proper rotations): 1, 2, 3, 4, 6
2. **Roto-inversion axes** (improper rotations): –1, –2, –3, –4, –6

The **rotation-inversion method is generally preferred** because:
- It provides a complete, unambiguous classification
- Roto-inversion axes naturally relate rotation + inversion (determinant = –1)
- The method generalizes consistently across all 32 classes

### Equivalences in Roto-Inversion Notation

- **–1** = Inversion center (pure inversion; identity rotation + inversion)
- **–2** = Equivalent to a mirror plane perpendicular to the 2-fold axis
- **–3, –4, –6** = Distinct improper rotation axes combining the respective rotations with inversion

### Generating Matrices Composition

For a point group with generators σ(i), the full group is obtained by:
- Taking all possible products (compositions): σ(i)·σ(j), σ(i)·σ(i), etc.
- Continuing until no new matrices appear

**Example relations** (from equations 2.5 in Birss):
$$\sigma^2 = -\sigma \cdot \sigma', \quad \sigma \cdot \sigma' \cdot \sigma = -\sigma', \quad \sigma^2 = \sigma'^2$$

These multiplication rules define the algebraic structure of the point group.

### Tensor Derivation from Constraints

Birss section 4 demonstrates the systematic procedure:

1. Write the constraint $\mathbf{d} = \sigma \cdot \mathbf{d}$ (for proper rotations) or $\mathbf{d} = -\sigma \cdot \mathbf{d}$ (for inversions)
2. For the generating matrices of a class, substitute each into the constraint
3. Solve for which coefficients must be equal or zero
4. The solution set gives the independent components

**For example (class 6/mmm, rank 4)**:
- Applying σ(1) (inversion): axial tensors vanish → only polar form
- Applying σ(2), σ(3): further restrictions reduce components to independent set
- Final result: specific number of independent coefficients (listed in Table 4f)

### Reference Materials

See **Section 11** ("Summary and Cross-References") for the full cross-reference
structure linking Table 3, Table 4a, Tables 4b–4f, and (for magnetic point groups)
Tables 6 and 7.


---

## 9. Axis and Index Conventions

### Index Ordering in Tensors
- Indices follow **x₁, x₂, x₃** (or **x, y, z**) in left-to-right order in the crystal frame
- In multicomponent notation (e.g., `xxyy`), indices are **read left to right**
- **Cyclic permutation** rotates indices in a cycle: `xyz → yzx → zxy → xyz`
  - Used in notations like `xxyz(c4)` (four cyclic permutations of component indices)
- **Restricted (non-cyclic) permutations** vary specific indices while preserving order of others
  - Example: `xxyy(x:3)` fixes the first index and permutes remaining indices

### Principal Axis Definition
See **Section 1** ("Crystal Coordinate System") for the per-crystal-system convention
for choosing x, y, z — which axis is the principal/unique axis, how the secondary axes
(`y` vs `x`) are assigned for tetragonal/trigonal/hexagonal classes, and how this
relates to Table 4a's "Orientation of reference axes" column.

### Crystal Frame vs. Stereographic Projection
- All coordinates $(x_1, x_2, x_3)$ in generating matrices are in the **crystal-fixed frame**.
- For the stereographic-projection conventions (equatorial projection, principal axis
  orientation, and the **●**/**○** above/below-plane markers), see **Section 1**.

---

## 10. Notation Summary Table

| Symbol/Notation | Meaning | Context | Reference |
|---|---|---|---|
| **σ(n)** | n-th generating matrix | Symmetry matrices | Table 3, column 8 |
| **E** or **1** | Identity operation | Symmetry operations | Base of all groups |
| **2_z** | 2-fold axis along z | Symmetry operations | Table 3, column 6 |
| **–2_z** | Mirror ⊥ to z (roto-inversion) | Symmetry operations | Table 3, column 6 |
| **2⊥** | 2-fold axis perpendicular to principal | Symmetry operations | Tables 3, 4c–4f |
| **–2⊥** | Mirror perpendicular to principal | Symmetry operations | Tables 3, 4c–4f |
| **3(2⊥)** | Three equivalent 2-fold axes ⊥ | Symmetry operations | Table 3 row D₃ |
| **3(–2⊥)** | Three mirrors ⊥ (in 3m class) | Symmetry operations | Table 3 row C₃ᵥ |
| **.** (dot) | Axis with parallel/containing mirror(s) | Shubnikov notation | `2.m`, `4.m`, `–6.m` |
| **:** (colon) | Axis with perpendicular mirror(s)/axes | Shubnikov notation | `2:m`, `4:2`, `m.2:m` |
| **/** (slash) | Cubic-only: [111]-type axes / [100]-type axes | Shubnikov notation | `3/2`, `–6/4` |
| **(3)** | Three unrestricted permutations | Tensor notation | Table 4e (e.g., `xxy(3)`) |
| **(x·3)** | Three permutations fixing last index | Tensor notation | Table 4f (e.g., `yxxx(x·3)`) |
| **(x:3)** | Three permutations fixing first index | Tensor notation | Table 4f (e.g., `xxyy(x:3)`) |
| **(c4)** | Four cyclic permutations | Tensor notation | Table 4f (e.g., `xxyz(c4)`) |
| **(xy:6)** | Six permutations preserving x,y order | Tensor notation | Table 4f (e.g., `zzxy(xy:6)`) |
| **0** | Component vanishes in this class | Tensor tables | Tables 4b–4f |
| **–n** (barred) | Barred n-fold roto-inversion axis | Symmetry operations (Table 3) | –1, –2, –3, –4, –6 in point group symbols |
| **–** in tensors | Minus sign coefficient on component | Tensor tables (Tables 4b–4f) | Indicates negative coefficient or inversion-odd component |
| **⊥** | Perpendicular symbol | Symmetry operations | Replaces book's perpendicular mark |

---

## 11. Summary and Cross-References

### Complete Reference Structure in Birss

The material in **Chapter 2** (scanned PDF pages 10–37, printed pages 1–55) establishes:

1. **Single crystal foundations** (scanned PDF pages 10–22, printed pages 1–25): Basic lattice structure, stereographic projections, symbol definitions
2. **Symmetry operations classification** (scanned PDF pages 23–25, printed pages 26–31): Proper vs. improper rotations, generating matrices, group composition
3. **Application methods** (scanned PDF pages 26–37, printed pages 32–55): Systematic tensor derivation, constraints from generators, tensor equalities between classes

### How to Use This Reference with the Tables

**To find tensor forms in a specific crystal class:**

1. Locate the **class in Table 3** (by international, Schoenflies, or Shubnikov symbol)
2. Extract the **generating matrices** from column 8
3. To understand what these matrices mean, use **Section 2** of this reference (generating matrices definitions)
4. Look up the class's row in **Table 4a** to find its **symbol class** for the rank you
   want: even rank m∈{0,2,4} → `A_m`...`U_m`, odd rank n∈{1,3} → `A_n`...`U_n`. See Table
   4a's "How to use this table" section for the full point-group → symbol-class lookup
   and rank mapping.
5. To see the resulting **tensor components**, go to the matching row (e.g. `H2`, `F4`)
   in the appropriate **Table 4b–4f** (rank 0–4)
6. To understand the **tensor notation** (why components are grouped, what numbers mean), use **Section 6** of this reference

**To understand symmetry operations in a specific class:**

1. Look at **Table 3, column 6** for the symmetry operations list
2. Use **Sections 2 and 4** to interpret each operation symbol (rotation vs. roto-inversion, meanings of ⊥, etc.)
3. Reference **Section 9** for axis conventions in that class

### Key Insight: Generating Matrices → Tensor Forms

The entire point of providing generating matrices is that they determine which tensor components survive in each class through the systematic constraint procedure outlined in **Section 5**. Tables 4a–4f are the **solutions** to these constraint equations, pre-computed for reference.

### The 122 Magnetic Point Groups: 𝒢, 𝒢′, and 𝓜

Birss Ch. 3, §2 (printed pp. 84–85) divides the 122 magnetic point groups into three
sets, according to how the time-reversal operator `R` (= `1'`) enters the group:

- **𝒢** (32, "classical groups", printed in **bold** in the book): `R` is not a
  symmetry operator at all — these are the ordinary 32 point groups of Table 3.
- **𝒢′** (32, "non-magnetic groups"): `R` is itself a symmetry operator, so
  `𝒢′ = 𝒢 ∪ R𝒢`. Birss writes these with the **same Hermann–Mauguin symbol as 𝒢**,
  distinguished only by typeface (non-bold) — these are the groups usually called the
  **"grey" groups** elsewhere in the literature.
- **𝓜** (58, "additional magnetic groups", black-and-white/primed): `R` occurs only
  combined with some of `𝒢`'s operators, via `M = H ∪ (G\H)'` (§13).

`32 + 32 + 58 = 122`.

**Tables 6 and 7 list only 90 rows — the 32 `𝒢` plus the 58 `𝓜`.** The 32 grey groups
`𝒢′` are not given separate rows, because for every `𝒢′`, `R` is itself a symmetry
operator, so:
- its i-tensor symbol class is identical to `𝒢`'s (the same-named, already-present
  type-I row of Table 7), and
- **every c-tensor is identically null** (a c-tensor changes sign under `R`, but
  `R ∈ 𝒢′` forces `d = -d`, i.e. `d = 0`) — this is rule **(a)** of §14.

A separate `𝒢′` row would therefore just repeat `𝒢`'s i-tensor columns with all
c-tensor columns blank, so Birss omits it.

### Extension to Magnetic Point Groups: Tables 6 and 7

**Table 6** lists the 90 magnetic point groups `𝒢` (32, type I, unprimed) and `𝓜` (58,
black-and-white) described above, using the same `σ(N)`/`σ'(N)` generating-matrix
notation (see **Sections 12–13** for the time-reversal/priming notation specific to
Table 6). The remaining 32 magnetic point groups — the grey groups `𝒢′` — are not
listed (see above).

**Table 7** extends Table 4a's 21-letter tensor-symbol-class scheme (`A_m`...`U_m`,
`A_n`...`U_n`) to the 90 magnetic point groups, giving each one an i-tensor and a
c-tensor symbol class. To go from a Table 7 symbol class to the actual tensor
components, apply Table 4a's rank mapping into Tables 4b–4f (m=0/2/4 → Tables 4b/4d/4f,
n=1/3 → Tables 4c/4e) — see Table 4a's "How to use this table" section for the full
lookup procedure.

**i-tensors vs. c-tensors**: for a magnetic point group with International symbol
`column 2`, let `G` = `unprime(column 2)` (the parent classical point group obtained by
dropping all primes, as in §13). A property tensor that is **invariant under time
reversal** ("i" for *invariant*) has the same form as it would in the classical group
`G` — its symbol class is simply **Table 4a's entry for `G`**. A property tensor that
**changes sign under time reversal** ("c" for *change of sign*, e.g. tensors relating
to magnetic moments) instead has its symbol class derived from Table 4a's entries for
the magnetic point group's two "Associated classical group" columns (A and B, Table 7
columns 3–4) via the cross-formula documented in table-7.md's "Notes and Status"
section. Table 7's columns 5–8 tabulate the i-tensor symbol classes and columns 9–12
the c-tensor symbol classes, for polar/axial tensors of even and odd rank.

---

## 12. Time-Reversal (Priming) Notation — Tables 6 and 7

### The Time-Reversal Operator and Primed Operations
- **1'** = the time-reversal (antisymmetry) operator (Birss Ch. 3, §2; eq. 3.15a–3.16b).
- A **primed operation** `g'` = the spatial symmetry operation `g` combined with time reversal.
- Magnetic point group symbols (Table 6, column 2) and their "Symmetry operators" lists (column 6)
  mark primed elements with a trailing `'`, e.g. `-1'`, `2'_z`, `m'`, `4'`, `±4'_z`, `±-3'_z`.

### Prime Placement on Ungrouped Operations
The prime is written immediately after the operation's rotation-order digit `N` — **after** any
leading roto-inversion marker (`-`, `±-`) but **before** any trailing axis subscript (`_z`, `_x`,
`_xy`, `_-xy`, ...) or `⊥`:

- `2'_z`, `-2'_z`, `-2'_xy`, `±4'_z`, `±-4'_z`, `±3'_z`, `±-3'_z`, `±6'_z`, `±-6'_z`
- `-1` (inversion) primes as `-1'`.

### Prime Placement on Grouped Operations `n(m...)`
In a grouped term `n(m...)` (see §4 and §7 for the `n(m)` / `n(m⊥)` grouping notation), `n` is a
**multiplicity count**, not an operation, and can never itself carry a prime. The prime belongs on
the operation symbol `m` inside the parentheses, in the **same position** as for ungrouped
operations (immediately after `m`'s rotation-order digit, before any trailing `⊥` or sign suffix):

| Correct | Incorrect |
|---|---|
| `6(2'⊥)` | `6'(2⊥)` |
| `3(-2'⊥)` | `3'(-2⊥)` |
| `3(±4')` | `3'(±4)` |
| `4(±-3')` | `4'(±-3)` |
| `9(-2')` | `9'(-2)` |
| `6(2')` | `6'(2)` |

This rule applies uniformly to the trigonal/hexagonal `n(m⊥)`/`n(-m⊥)` families and the cubic
`n(m)`/`n(-m)`/`n(±m)`/`n(±-m)` families (§7).

### Magnetic Shubnikov Notation
Primes appear analogously in Shubnikov symbols, marking the primed generator/coset, e.g. `4':2`,
`m'.6:m'`, `-6'/4'`.

---

## 13. Deriving Black-and-White Magnetic Point Group Operation Lists: M = H ∪ (G\H)'

For the primed rows of Table 6 (those whose "Classical subgroup (International)" entry, column 4,
is not `-`), the "Symmetry operators" column (column 6) can be derived — and cross-checked —
purely from Table 3, independent of the row's symbol primes or its generating-matrix columns:

- **G** = `unprime(column 2)` — drop all primes from the magnetic point group's International
  symbol to get its parent classical (unprimed) point group. G's operation list is Table 3's
  "Symmetry operations" entry for G.
- **H** = column 4, "Classical subgroup (International)" — an index-2 subgroup of G. H's operation
  list is likewise Table 3's entry for H.
- **M** (column 6) = `H ∪ (G\H)'`, i.e. all of H's operations unprimed, plus every operation in G
  but not in H, each combined with time reversal (primed per §12 above).

### Sanity Check
`unprime(M)` (drop every prime from M) must reproduce G's full Table 3 operation multiset exactly,
and `|M| = |G| = 2|H|`. This catches both element-set errors and prime-placement errors.

### Computing G\H via Atomic Operation Families
Table 3 groups several equivalent operations into single terms (e.g. `3(2⊥)`, `9(2)`, `4(±3)`).
Because H's grouped term may represent only *part* of G's, G\H must generally be computed by
decomposing each system's grouped terms into "atomic operation families" and subtracting counts,
not by literal term subtraction:

- **Triclinic/Monoclinic/Orthorhombic/Tetragonal**: every Table 3 term is already a singleton or an
  atomic pair (`±4_z`/`±-4_z` and `±-4_z`/`±4_z` always travel together as a pair). G\H is a plain
  set difference of terms.
- **Trigonal/Hexagonal**: the relevant families are `2⊥` and `-2⊥`, each occurring with a count of
  0, 3, or 6 depending on the group. `6(X⊥) − 3(X⊥) = 3(X⊥)` (same family label, reduced count) —
  valid because H's 3 axes of type `X⊥` are a literal subset of G's 6.
- **Cubic**: the relevant families are:
  - `2_coord`/`-2_coord` (≤3): 2-fold rotations/mirrors about the 3 coordinate axes — the same axes
    that, when 4-fold symmetry is present, also host the `±4`/`±-4` operations.
  - `2_facediag`/`-2_facediag` (≤6): 2-fold rotations/mirrors about the 6 face-diagonal axes.
  - `±3`/`±-3` (≤4): 3-fold rotations/roto-inversions about the 4 body-diagonal axes — Table 3's
    `4(±3)`/`4(±-3)` terms.
  - `±4`/`±-4` (≤3): 4-fold rotations/roto-inversions about the 3 coordinate axes — Table 3's
    `3(±4)`/`3(±-4)` terms.
  - Table 3's combined `9(2)`/`9(-2)` terms decompose as `2_coord`(3) + `2_facediag`(6).

### Worked Example
For magnetic point group `4'32'` (Table 6, H = `23`):
- G = `432` = `1, 9(2), 4(±3), 3(±4)` (24 operations).
- H = `23` = `1, 3(2), 4(±3)` (12 operations), where H's `3(2)` is the `2_coord`(3) part of G's
  `9(2)`.
- G\H = `9(2) − 3(2) = 6(2)` (the `2_facediag`(6) remainder), plus `3(±4)` (absent from H entirely).
- `(G\H)' = 6(2'), 3(±4')`.
- M = H ∪ (G\H)' = `1, 3(2), 4(±3), 6(2'), 3(±4')` — matching Table 6's entry for `4'32'`.

---

## 14. Null Property Tensors: "Forbidden" Effects

This section summarizes Birss's discussion of which tensor properties are identically
zero ("forbidden" effects) in which crystal classes: Chapter 2, §7 (printed pp. 71–73)
for the 32 classical point groups, and Chapter 3, §5 (printed pp. 122–124) for the 90
magnetic point groups.

### Classical Point Groups (Ch. 2, §7)

**Rank > 2**: For tensors of rank greater than the third, the *only* restriction
imposed by spatial symmetry is the centrosymmetric rule already given in §5/§7 above:
in the 11 centrosymmetric classes (`-1, 2/m, mmm, 4/m, 4/mmm, -3, -3m, 6/m, 6/mmm, m3,
m3m`), polar tensors of odd rank and axial tensors of even rank vanish identically;
otherwise no general nullity is imposed by symmetry. The same rule covers general
third-rank tensors too, although for a *particular* third-rank tensor,
particularization by intrinsic (index) symmetry can additionally force it to vanish in
a non-centrosymmetric class — e.g. the piezomagnetic tensor component $H_3 = 0$ for
class `422`.

**Rank 2 (general tensor, not assuming intrinsic symmetry)**:
- A general second-rank **polar** tensor (e.g. permittivity) is never forced to zero
  by symmetry in *any* of the 32 classes.
- A general second-rank **axial** tensor (e.g. the optical gyration tensor) vanishes
  identically in the 11 centrosymmetric classes, **and additionally** in `-6, -6m2,
  -43m` — these three classes have Table 4a "Axial tensor of even rank m" symbol
  classes `O_m`, `R_m`, `U_m`, and rows `O2`, `R2`, `U2` in Table 4d are all-zero. 14
  classes in total therefore exhibit no general second-rank axial-tensor properties
  (e.g. no piezomagnetism).

**Rank 1 (polar and axial vectors — pyroelectricity and pyromagnetism)**:
- A **polar vector** (pyroelectricity) is forbidden in the 11 centrosymmetric classes
  and additionally in `222, -4, 422, -42m, 32, -6, 622, -6m2, 23, 432, -43m` — these 11
  classes have Table 4a "Polar tensor of odd rank n" symbol classes `D_n, G_n, H_n,
  J_n, L_n, O_n, P_n, R_n, S_n, T_n, U_n`, and rows `D1, G1, H1, J1, L1, O1, P1, R1, S1,
  T1, U1` in Table 4c are all `0, 0, 0`. 22 classes in total forbid pyroelectricity;
  the remaining **10** classes — `1, 2, m, mm2, 4, 4mm, 3, 3m, 6, 6mm` — permit it
  (the 10 polar point groups).
- An **axial vector** (pyromagnetism) is permitted **only** in the 13 classes `1, -1,
  2, m, 2/m, 4, -4, 4/m, 3, -3, 6, -6, 6/m` — these have Table 4a "Axial tensor of odd
  rank n" symbol classes `A_n, B_n, F_n, K_n, N_n`, whose Table 4c rows (`A1`, `B1`,
  `F1`, `K1`, `N1`) have a nonzero `z` component. In the remaining 19 classes,
  pyromagnetism is forbidden.

**i-tensors and c-tensors**: Curie [1908] and Voigt [1928] unsuccessfully tried to
demonstrate pyromagnetism experimentally; Zocher and Török [1953] then argued that
pyromagnetism is universally "forbidden" by symmetry. Their argument rests on dividing
property tensors, by their behavior under time-inversion, into **i-tensors**
(invariant under time reversal) and **c-tensors** (change sign under time reversal —
see §11). Since magnetic moment is time-antisymmetric, pyro- and piezomagnetism are
characterized by c-tensors, and Zocher and Török assumed *all* crystals are
time-symmetric, so that *all* c-tensors must vanish. Birss's rebuttal — and the
motivation for the magnetic-point-group treatment below — is that this assumption
holds only for diamagnetic/paramagnetic materials (no magnetic order, time-reversal an
exact symmetry); ferro-, ferri-, and antiferromagnetic crystals are *not*
time-symmetric, so their c-tensors need not vanish, and the rank-1/rank-2 results above
(derived purely from spatial symmetry) become the operative "forbidden" conditions.

### Magnetic Point Groups (Ch. 3, §5)

For a magnetic point group, every property tensor is classified (§11) as an
**i-tensor** (Table 7 columns 5–8, depending only on the parent classical group `G`)
or a **c-tensor** (Table 7 columns 9–12, derived from the "Associated classical
groups" A and B). For *static* properties, Birss gives five nullity rules:

- **(a)** For materials with **no magnetic order** (described by the 32 classical
  point groups `𝒢′`, for which time-reversal `1'` is an exact symmetry operation),
  **all c-tensors vanish identically** — this is the physical statement underlying the
  rebuttal above: it is the *magnetically ordered* crystal's magnetic point group, not
  `𝒢′`, that determines via rules (b)–(e) below whether a c-tensor is null.
- **(b)** For the 11 centrosymmetric classical groups (set `n₁`, eq. 3.47 — the same
  11 classes listed above: `-1, 2/m, mmm, 4/m, 4/mmm, -3, -3m, 6/m, 6/mmm, m3, m3m`),
  **polar i-tensors of odd rank and axial i-tensors of even rank vanish identically**
  — the same centrosymmetric rule, now applied to the i-tensor of any magnetic point
  group whose parent `G` is in `n₁`.

Within the 90 magnetic point groups (Table 7), two further 21-member subsets `m₂` and
`m₃` are defined (eqs. 3.48–3.49):
- `m₂` = the rows of Table 7 whose c-tensor "Axial tensor of even rank m" (column 10)
  and "Polar tensor of odd rank n" (column 11) entries are *both* blank:
  `-1, 2/m, 2'/m', mmm, m'm'm, 4/m, 4'/m, 4/mmm, 4'/mmm', 4/mm'm', -3, -3m, -3m', 6/m,
  6'/m', 6/mmm, 6'/mmm', 6/mm'm', m3, m3m, m3m'`
- `m₃` = the rows of Table 7 whose c-tensor "Polar tensor of even rank m" (column 9)
  and "Axial tensor of odd rank n" (column 12) entries are *both* blank:
  `-1', 2/m', 2'/m, m'm'm', mmm', 4/m', 4'/m', 4/m'm'm', 4/m'mm, 4'/m'm'm, -3', -3'm',
  -3'm, 6/m', 6'/m, 6/m'm'm', 6/m'mm, 6'/mm'm, m'3, m'3m', m'3m`

`m₁ = m₂ + m₃` (42 classes) comprises exactly the magnetic point groups that are, or
are derived from, the centrosymmetric classical classes `n₁`. The remaining rules are:

- **(c)** Axial c-tensors of even rank and polar c-tensors of odd rank are null in the
  21 magnetic crystal classes of `m₂`.
- **(d)** Polar c-tensors of even rank and axial c-tensors of odd rank are null in the
  21 magnetic crystal classes of `m₃`.
- **(e)** Axial i-tensors of even rank and polar i-tensors of odd rank are null in the
  42 magnetic crystal classes of `m₁ = m₂ + m₃`.

The detailed application of (a)–(e) to specific effects — analogous to the
pyroelectricity/pyromagnetism discussion above, but for magnetically ordered crystals
— is carried out in Birss Chapters 4 and 5 (ferro-/ferrimagnetic and antiferromagnetic
materials).

