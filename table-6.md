# Table 6: The 122 Magnetic Point Groups

Source: scanned PDF pages 55-59 in `Birss Symmetry & Magnetism komplett.pdf`
(printed book pages 91-98; the table is printed rotated by 90 degrees and spans these
8 printed pages across 5 scanned-PDF pages)

**Note**: Of the 122 magnetic point groups, this table lists only the 90 that carry independent information: the 32 classical (type I, unprimed) groups and the 58 black-and-white (type III, primed) groups. The remaining 32 "grey" (type II) groups are omitted — each is trivially derived from its classical counterpart (same i-tensor; every c-tensor vanishes identically; see `conventions-reference.md` §12 and §15, rule (a)).

**How to use this table / how it connects to the others**: this table has the same
column layout as Table 3 (point-group symbol, symmetry operators, generating matrices
`σ(N)`/`σ'(N)`), extended with a "Classical subgroup" column for the 90
black-and-white (primed) magnetic point groups. To find the i-/c-tensor symbol classes
(and hence the tensor forms in Tables 4a-4f) for a magnetic point group listed here, look
up its row in Table 7.

---

## Opening Subsection: Triclinic and Monoclinic Groups

The first block of Table 6, on printed page 91 (scanned PDF pages 55-56), covers the triclinic and monoclinic magnetic point groups. The book uses the same overall structure as Table 3, with the magnetic point-group symbol, the classical subgroup, the symmetry operators of the magnetic group, and the generating matrices listed in separate columns. In this transcription, inversion is written with `-` and time reversal with `'`.

**Notation and derivation**: see `conventions-reference.md` §13 for the time-reversal prime notation
(including the prime-placement rule for grouped terms `n(m')`, not `n'(m)`), and §14 for the
`M = H ∪ (G\H)'` formula used to derive/verify the "Symmetry operators" column for the
black-and-white (primed) rows from Table 3.

| System | Magnetic point group (International) | Magnetic point group (Shubnikov) | Classical subgroup (International) | Classical subgroup (Shubnikov) | Symmetry operators | Generating matrices of subgroup | Additional generating matrix |
|---|---|---|---|---|---|---|---|
| Triclinic | 1 | 1 | - | - | 1 | σ(0) | - |
| Triclinic | -1 | -2 | - | - | 1, -1 | σ(1) | - |
| Triclinic | -1' | -2' | 1 | 1 | 1, -1' | σ(0) | σ'(1) |
| Monoclinic | 2 | 2 | - | - | 1, 2_z | σ(3) | - |
| Monoclinic | 2' | 2' | 1 | 1 | 1, 2'_z | σ(0) | σ'(3) |
| Monoclinic | m | m | - | - | 1, -2_z | σ(5) | - |
| Monoclinic | m' | m' | 1 | 1 | 1, -2'_z | σ(0) | σ'(5) |
| Monoclinic | 2/m | 2:m | - | - | 1, -1, 2_z, -2_z | σ(1), σ(3) | - |
| Monoclinic | 2'/m' | 2':m' | -1 | -2 | 1, -1, 2'_z, -2'_z | σ(1) | σ'(3) |
| Monoclinic | 2/m' | 2:m' | 2 | 2 | 1, 2_z, -1', -2'_z | σ(3) | σ'(1) |
| Monoclinic | 2'/m | 2':m | m | m | 1, -2_z, -1', 2'_z | σ(5) | σ'(1) |
| Orthorhombic | 222 | 2:2 | - | - | 1, 2_x, 2_y, 2_z | σ(2), σ(3) | - |
| Orthorhombic | 2'2'2 | 2:2' | 2 | 2 | 1, 2_z, 2'_x, 2'_y | σ(3) | σ'(2) |
| Orthorhombic | mm2 | 2.m | - | - | 1, 2_z, -2_x, -2_y | σ(3), σ(4) | - |
| Orthorhombic | m'm'2 | 2.m' | 2 | 2 | 1, 2_z, -2'_x, -2'_y | σ(3) | σ'(4) |
| Orthorhombic | 2'm'm | 2'.m | m | m | 1, -2_z, 2'_x, -2'_y | σ(5) | σ'(4) |
| Orthorhombic | mmm | m.2:m | - | - | 1, -1, 2_x, 2_y, 2_z, -2_x, -2_y, -2_z | σ(1), σ(2), σ(3) | - |
| Orthorhombic | m'm'm | m'.2:m | 2/m | 2:m | 1, -1, 2_z, -2_z, 2'_x, 2'_y, -2'_x, -2'_y | σ(1), σ(3) | σ'(2) |
| Orthorhombic | m'm'm' | m'.2:m' | 222 | 2:2 | 1, 2_x, 2_y, 2_z, -1', -2'_x, -2'_y, -2'_z | σ(2), σ(3) | σ'(1) |
| Orthorhombic | mmm' | m.2:m' | mm2 | 2.m | 1, 2_z, -2_x, -2_y, -1', 2'_x, 2'_y, -2'_z | σ(3), σ(4) | σ'(1) |
| Tetragonal | 4 | 4 | - | - | 1, 2_z, ±4_z | σ(7) | - |
| Tetragonal | 4' | 4' | 2 | 2 | 1, 2_z, ±4'_z | σ(3) | σ'(7) |
| Tetragonal | -4 | -4 | - | - | 1, 2_z, ±-4_z | σ(8) | - |
| Tetragonal | -4' | -4' | 2 | 2 | 1, 2_z, ±-4'_z | σ(3) | σ'(8) |
| Tetragonal | 4/m | 4:m | - | - | 1, -1, 2_z, -2_z, ±4_z, ±-4_z | σ(1), σ(7) | - |
| Tetragonal | 4'/m | 4':m | 2/m | 2:m | 1, -1, 2_z, -2_z, ±4'_z, ±-4'_z | σ(1), σ(3) | σ'(7) |
| Tetragonal | 4/m' | 4:m' | 4 | 4 | 1, 2_z, ±4_z, -1', -2'_z, ±-4'_z | σ(7) | σ'(1) |
| Tetragonal | 4'/m' | 4':m' | -4 | -4 | 1, 2_z, ±-4_z, -1', -2'_z, ±4'_z | σ(8) | σ'(1) |
| Tetragonal | 422 | 4:2 | - | - | 1, 2_x, 2_y, 2_z, 2_xy, 2_-xy, ±4_z | σ(2), σ(7) | - |
| Tetragonal | 4'22' | 4':2 | 222 | 2:2 | 1, 2_x, 2_y, 2_z, 2'_xy, 2'_-xy, ±4'_z | σ(2), σ(3) | σ'(7) |
| Tetragonal | 42'2' | 4:2' | 4 | 4 | 1, 2_z, ±4_z, 2'_x, 2'_y, 2'_xy, 2'_-xy | σ(7) | σ'(2) |
| Tetragonal | 4mm | 4.m | - | - | 1, 2_z, -2_x, -2_y, -2_xy, -2_-xy, ±4_z | σ(4), σ(7) | - |
| Tetragonal | 4'mm' | 4'.m | mm2 | 2.m | 1, 2_z, -2_x, -2_y, -2'_xy, -2'_-xy, ±4'_z | σ(3), σ(4) | σ'(7) |
| Tetragonal | 4m'm' | 4.m' | 4 | 4 | 1, 2_z, ±4_z, -2'_x, -2'_y, -2'_xy, -2'_-xy | σ(7) | σ'(4) |
| Tetragonal | -42m | -4.m | - | - | 1, 2_x, 2_y, 2_z, -2_xy, -2_-xy, ±-4_z | σ(2), σ(8) | - |
| Tetragonal | -4'2m' | -4'.m' | 222 | 2:2 | 1, 2_x, 2_y, 2_z, -2'_xy, -2'_-xy, ±-4'_z | σ(2), σ(3) | σ'(8) |
| Tetragonal | -4'm2' | -4'.m | mm2 | 2.m | 1, 2_z, -2_x, -2_y, 2'_xy, 2'_-xy, ±-4'_z | σ(3), σ(4) | σ'(8) |
| Tetragonal | -42'm' | -4.m' | -4 | -4 | 1, 2_z, ±-4_z, 2'_x, 2'_y, -2'_xy, -2'_-xy | σ(8) | σ'(2) |
| Tetragonal | 4/mmm | m.4:m | - | - | 1, -1, 2_x, 2_y, 2_z, 2_xy, 2_-xy, -2_x, -2_y, -2_z, -2_xy, -2_-xy, ±4_z, ±-4_z | σ(1), σ(2), σ(7) | - |
| Tetragonal | 4'/mmm' | m.4':m | mmm | m.2:m | 1, -1, 2_x, 2_y, 2_z, -2_x, -2_y, -2_z, 2'_xy, 2'_-xy, -2'_xy, -2'_-xy, ±4'_z, ±-4'_z | σ(1), σ(2), σ(3) | σ'(7) |
| Tetragonal | 4/mm'm' | m.4:m' | 4/m | 4:m | 1, -1, 2_z, -2_z, ±4_z, ±-4_z, 2'_x, 2'_y, 2'_xy, 2'_-xy, -2'_x, -2'_y, -2'_xy, -2'_-xy | σ(1), σ(7) | σ'(2) |
| Tetragonal | 4/m'm'm' | m'.4:m' | 422 | 4:2 | 1, 2_x, 2_y, 2_z, 2_xy, 2_-xy, ±4_z, -1', -2'_x, -2'_y, -2'_z, -2'_xy, -2'_-xy, ±-4'_z | σ(2), σ(7) | σ'(1) |
| Tetragonal | 4/m'mm | m'.4:m | 4mm | 4.m | 1, 2_z, -2_x, -2_y, -2_xy, -2_-xy, ±4_z, -1', 2'_x, 2'_y, -2'_z, 2'_xy, 2'_-xy, ±-4'_z | σ(4), σ(7) | σ'(1) |
| Tetragonal | 4'/m'm'm | m'.4':m' | -42m | -4.m | 1, 2_x, 2_y, 2_z, -2_xy, -2_-xy, ±-4_z, -1', -2'_x, -2'_y, -2'_z, 2'_xy, 2'_-xy, ±4'_z | σ(2), σ(8) | σ'(1) |
| Trigonal | 3 | 3 | - | - | 1, ±3_z | σ(6) | - |
| Trigonal | -3 | -6 | - | - | 1, -1, ±3_z, ±-3_z | σ(1), σ(6) | - |
| Trigonal | -3' | -6' | 3 | 3 | 1, ±3_z, -1', ±-3'_z | σ(6) | σ'(1) |
| Trigonal | 32 | 3:2 | - | - | 1, 3(2⊥), ±3_z | σ(2), σ(6) | - |
| Trigonal | 32' | 3:2' | 3 | 3 | 1, ±3_z, 3(2'⊥) | σ(6) | σ'(2) |
| Trigonal | 3m | 3.m | - | - | 1, 3(-2⊥), ±3_z | σ(4), σ(6) | - |
| Trigonal | 3m' | 3.m' | 3 | 3 | 1, ±3_z, 3(-2'⊥) | σ(6) | σ'(4) |
| Trigonal | -3m | -6.m | - | - | 1, -1, 3(2⊥), 3(-2⊥), ±3_z, ±-3_z | σ(1), σ(2), σ(6) | - |
| Trigonal | -3m' | -6.m' | -3 | -6 | 1, -1, ±3_z, ±-3_z, 3(2'⊥), 3(-2'⊥) | σ(1), σ(6) | σ'(2) |
| Trigonal | -3'm' | -6'.m' | 32 | 3:2 | 1, 3(2⊥), ±3_z, -1', 3(-2'⊥), ±-3'_z | σ(2), σ(6) | σ'(1) |
| Trigonal | -3'm | -6'.m | 3m | 3.m | 1, ±3_z, 3(-2⊥), -1', 3(2'⊥), ±-3'_z | σ(4), σ(6) | σ'(1) |
| Hexagonal | 6 | 6 | - | - | 1, 2_z, ±3_z, ±6_z | σ(3), σ(6) | - |
| Hexagonal | 6' | 6' | 3 | 3 | 1, ±3_z, 2'_z, ±6'_z | σ(6) | σ'(3) |
| Hexagonal | -6 | 3:m | - | - | 1, -2_z, ±3_z, ±-6_z | σ(5), σ(6) | - |
| Hexagonal | -6' | 3:m' | 3 | 3 | 1, ±3_z, -2'_z, ±-6'_z | σ(6) | σ'(5) |
| Hexagonal | 6/m | 6:m | - | - | 1, -1, 2_z, -2_z, ±3_z, ±-3_z, ±6_z, ±-6_z | σ(1), σ(3), σ(6) | - |
| Hexagonal | 6'/m' | 6':m' | -3 | -6 | 1, -1, ±3_z, ±-3_z, 2'_z, -2'_z, ±6'_z, ±-6'_z | σ(1), σ(6) | σ'(3) |
| Hexagonal | 6/m' | 6:m' | 6 | 6 | 1, 2_z, ±3_z, ±6_z, -1', -2'_z, ±-3'_z, ±-6'_z | σ(3), σ(6) | σ'(1) |
| Hexagonal | 6'/m | 6':m | -6 | 3:m | 1, -2_z, ±3_z, ±-6_z, -1', 2'_z, ±-3'_z, ±6'_z | σ(5), σ(6) | σ'(1) |
| Hexagonal | 622 | 6:2 | - | - | 1, 6(2⊥), 2_z, ±3_z, ±6_z | σ(2), σ(3), σ(6) | - |
| Hexagonal | 6'22' | 6':2 | 32 | 3:2 | 1, 3(2⊥), ±3_z, 3(2'⊥), 2'_z, ±6'_z | σ(2), σ(6) | σ'(3) |
| Hexagonal | 62'2' | 6:2' | 6 | 6 | 1, 2_z, ±3_z, ±6_z, 6(2'⊥) | σ(3), σ(6) | σ'(2) |
| Hexagonal | 6mm | 6.m | - | - | 1, 2_z, 6(-2⊥), ±3_z, ±6_z | σ(3), σ(4), σ(6) | - |
| Hexagonal | 6'mm' | 6'.m | 3m | 3.m | 1, 3(-2⊥), ±3_z, 2'_z, ±6'_z, 3(-2'⊥) | σ(4), σ(6) | σ'(3) |
| Hexagonal | 6m'm' | 6.m' | 6 | 6 | 1, 2_z, ±3_z, ±6_z, 6(-2'⊥) | σ(3), σ(6) | σ'(4) |
| Hexagonal | -6m2 | m.3:m | - | - | 1, 3(2⊥), 3(-2⊥), -2_z, ±3_z, ±-6_z | σ(4), σ(5), σ(6) | - |
| Hexagonal | -6'2m' | m'.3:m' | 32 | 3:2 | 1, 3(2⊥), ±3_z, -2'_z, ±-6'_z, 3(-2'⊥) | σ(2), σ(6) | σ'(5) |
| Hexagonal | -6'm2' | m.3:m' | 3m | 3.m | 1, 3(-2⊥), ±3_z, 3(2'⊥), -2'_z, ±-6'_z | σ(4), σ(6) | σ'(5) |
| Hexagonal | -6m'2' | m'.3:m | -6 | 3:m | 1, -2_z, ±3_z, ±-6_z, 3(2'⊥), 3(-2'⊥) | σ(5), σ(6) | σ'(4) |
| Hexagonal | 6/mmm | m.6:m | - | - | 1, -1, 6(2⊥), 2_z, 6(-2⊥), -2_z, ±3_z, ±-3_z, ±6_z, ±-6_z | σ(1), σ(2), σ(3), σ(6) | - |
| Hexagonal | 6'/m'mm' | m'.6':m' | -3m | -6.m | 1, -1, 3(2⊥), 3(-2⊥), ±3_z, ±-3_z, 3(2'⊥), 2'_z, 3(-2'⊥), -2'_z, ±6'_z, ±-6'_z | σ(1), σ(2), σ(6) | σ'(3) |
| Hexagonal | 6/mm'm' | m'.6:m | 6/m | 6:m | 1, -1, 2_z, -2_z, ±3_z, ±-3_z, ±6_z, ±-6_z, 6(2'⊥), 6(-2'⊥) | σ(1), σ(3), σ(6) | σ'(2) |
| Hexagonal | 6/m'm'm' | m'.6:m' | 622 | 6:2 | 1, 6(2⊥), 2_z, ±3_z, ±6_z, -1', -2'_z, ±-3'_z, ±-6'_z, 6(-2'⊥) | σ(2), σ(3), σ(6) | σ'(1) |
| Hexagonal | 6/m'mm | m.6:m' | 6mm | 6.m | 1, 2_z, 6(-2⊥), ±3_z, ±6_z, -1', -2'_z, 6(2'⊥), ±-3'_z, ±-6'_z | σ(3), σ(4), σ(6) | σ'(1) |
| Hexagonal | 6'/mm'm | m.6':m | -6m2 | m.3:m | 1, 3(2⊥), 3(-2⊥), -2_z, ±3_z, ±-6_z, -1', 2'_z, 3(2'⊥), 3(-2'⊥), ±-3'_z, ±6'_z | σ(4), σ(5), σ(6) | σ'(1) |
| Cubic | 23 | 3/2 | - | - | 1, 3(2), 4(±3) | σ(3), σ(9) | - |
| Cubic | m3 | -6/2 | - | - | 1, -1, 3(2), 3(-2), 4(±3), 4(±-3) | σ(1), σ(3), σ(9) | - |
| Cubic | m'3 | -6'/2 | 23 | 3/2 | 1, 3(2), 4(±3), -1', 3(-2'), 4(±-3') | σ(3), σ(9) | σ'(1) |
| Cubic | 432 | 3/4 | - | - | 1, 9(2), 4(±3), 3(±4) | σ(7), σ(9) | - |
| Cubic | 4'32' | 3/4' | 23 | 3/2 | 1, 3(2), 4(±3), 6(2'), 3(±4') | σ(3), σ(9) | σ'(7) |
| Cubic | -43m | 3/-4 | - | - | 1, 3(2), 6(-2), 4(±3), 3(±-4) | σ(8), σ(9) | - |
| Cubic | -4'3m' | 3/-4' | 23 | 3/2 | 1, 3(2), 4(±3), 6(-2'), 3(±-4') | σ(3), σ(9) | σ'(8) |
| Cubic | m3m | -6/4 | - | - | 1, -1, 9(2), 9(-2), 4(±3), 4(±-3), 3(±4), 3(±-4) | σ(1), σ(7), σ(9) | - |
| Cubic | m3m' | -6/4' | m3 | -6/2 | 1, -1, 3(2), 3(-2), 4(±3), 4(±-3), 6(2'), 6(-2'), 3(±4'), 3(±-4') | σ(1), σ(3), σ(9) | σ'(7) |
| Cubic | m'3m' | -6'/4' | 432 | 3/4 | 1, 9(2), 4(±3), 3(±4), -1', 9(-2'), 4(±-3'), 3(±-4') | σ(7), σ(9) | σ'(1) |
| Cubic | m'3m | -6'/4 | -43m | 3/4 | 1, 3(2), 6(-2), 4(±3), 3(±-4), -1', 3(-2'), 6(2'), 4(±-3'), 3(±4') | σ(8), σ(9) | σ'(1) |

---

## Status and Known Open Issues

The table above covers all seven crystal systems (90 rows). Per Birss (Ch. 3, §2), the 122 magnetic
point groups consist of three sets: the 32 classical groups `𝒢` (type I, unprimed, bold-face in the
book), the 32 "non-magnetic"/grey groups `𝒢′` (type II — same Hermann-Mauguin symbol as `𝒢`, non-bold,
with time-reversal `R`=`1'` itself a symmetry operator), and the 58 additional (black-and-white,
primed) magnetic groups `𝓜` (type III). This table lists the 90 rows comprising `𝒢` (32, "Classical
subgroup" = `-`) and `𝓜` (58); the 32 grey groups `𝒢′` are omitted, since for each of them the
i-tensor is identical to the same-named `𝒢` row and every c-tensor vanishes identically (see
`conventions-reference.md` §12 and §15, rule (a)).

**2026-06 verification pass (complete)**: All 90 rows have been cross-checked column-by-column
(Classical subgroup International/Shubnikov, Symmetry operators, Generating matrices of subgroup,
Additional generating matrix) against Table 3, against the M = H ∪ (G\H)' group-theory structure
(H = Classical subgroup, G = unprime of column 2, |H| = |G\H| = |G|/2), and against the source page
images (scanned PDF pages 55-59 = printed pages 91-98, OCR crops in `.tmp_ocr/`). Column 2 (Magnetic point group, International) was
left untouched throughout, per standing instruction — it was already correct and fixed.

Notable fixes made during this pass:
- Tetragonal (41-64): corrected several Shubnikov/classical-subgroup pairings, symmetry-operator
  primes, and generator/additional-generator entries (e.g. the `-4`-subgroup row's generators, which
  had incorrectly mirrored a `4mm`-type row).
- Trigonal (65-75): corrected classical-subgroup Shubnikov symbols and operator primes for the `-3'`,
  `-3m'`, `-3'm'`, `-3'm` rows.
- Hexagonal (76-99): corrected a cyclic mis-assignment of classical subgroups across rows 97-99
  (`622`/`6mm`/`-6m2` had been rotated), fixed missing/incorrect primes throughout the `6/m`, `622`,
  `6mm`, `-6m2`, and `6/mmm` families, and established systematic priming rules for the `6/mmm` family's
  Shubnikov slots. Row 91 (`-6'2m'`) is the bracketed/rotated-axis special case noted in Table 7's
  header note; its columns 3-8 were transcribed directly from the source image (`hex_6m2_cols23.png`)
  rather than derived, due to the axis-convention ambiguity.
- Cubic (100-110): fixed Shubnikov symbols for the four BW rows (`m'3`→`-6'/2`, `4'32'`→`3/4'`,
  `-4'3m'`→`3/-4'`, `m3m'`→`-6/4'`, `m'3m'`→`-6'/4'`, `m'3m`→`-6'/4`, transcribed from
  `cubic_p58_col23_zoom.png`/`cubic_p59_col23_*.png`), corrected the `4'32'`/`-4'3m'`/`m3m'` symmetry-
  operator lists to prime the G\H elements, fixed `m'3m`'s sign on the `6(2)`/`-6(2)` terms, and
  corrected three additional-generator entries (`4'32'`→`σ'(7)`, `-4'3m'`→`σ'(8)`, `m3m'`→`σ'(7)`) and
  one generator-of-subgroup entry (`m'3m'`'s `σ(2),σ(9)`→`σ(7),σ(9)`, matching `432`'s Table 3
  generators), all confirmed against `cubic_col8_*.png`.

**2026-06 pass 2 (32 unprimed `𝒢` rows vs. updated Table 3 notation)**: Table 3's symmetry-operation
notation was subsequently revised (`±-n_z` for roto-inversion pairs, `n(m⊥)`/`n(-m⊥)` for
trigonal/hexagonal groupings, `n(m)`/`n(-m)` infix-minus for cubic groupings, `2_xy`/`2_-xy` for
tetragonal diagonal axes). Re-checked all 32 unprimed `𝒢` rows (Classical subgroup = `-`; not to be
confused with the omitted grey `𝒢′` groups, see "Status and Known Open Issues" above) against Table
3's "Symmetry operations" column under this notation and fixed:
- `4mm` (row 52): `2_xy` → `-2_xy` (content error — 4mm/C4v has no proper diagonal 2-fold, only
  diagonal mirrors).
- `4/mmm` (row 59): reordered `±-4_z, ±4_z` → `±4_z, ±-4_z` to match Table 3 (same element set).
- `-6m2` (row 90): `±6_z` → `±-6_z` (content error — D3h/-6m2 contains S3 roto-inversions, not C6
  rotations) and `3(2), -3(2)` → `3(2⊥), 3(-2⊥)` (notation).
- `-43m` (row 105): `3(±4)` → `3(±-4)` (content error — Td/-43m contains S4 roto-inversions, not C4
  rotations) and `-6(2)` → `6(-2)` (notation).
- Trigonal/hexagonal `n(m)`/`n(-m)` groupings updated to `n(m⊥)`/`n(-m⊥)`: `32` (68), `3m` (70), `-3m`
  (72), `622` (84), `6mm` (87), `6/mmm` (94).
- Cubic prefix-minus groupings updated to infix-minus: `m3` (101) `3(2), -3(2), 4(±3), -4(±3)` →
  `3(2), 3(-2), 4(±3), 4(±-3)`; `m3m` (107) `9(-2)→9(2)`-style terms → `9(2), 9(-2), ..., 3(±4),
  3(±-4)`.

**Open follow-up (resolved by pass 3 below)**: the three content fixes above (`-6m2`'s `±-6_z` and
`-43m`'s `3(±-4)`) and the `n(m⊥)`/infix-minus notation changes are mirrored in several
black-and-white (primed) rows that share the same classical subgroup H (rows 74, 75, 85, 88, 91, 92,
95, 97, 98, 99 for the trigonal/hexagonal `n(m)`→`n(m⊥)` notation; rows 102, 106 for `-43m`'s
`3(±4)`→`3(±-4)`-type content).

**2026-06 pass 3 (58 black-and-white rows, derivation from Table 3 by set arithmetic)**: For every
BW (type III) row, M = H ∪ (G\H)' was derived purely from Table 3's operation lists for G (= unprime
of column 2) and H (= column 4, "Classical subgroup"), using per-system "atomic operation family"
arithmetic (plain set difference for tri/mono/ortho/tetragonal; `2⊥`/`-2⊥` families with counts 3/6
for trigonal/hexagonal; `2_coord`/`-2_coord`/`2_facediag`/`-2_facediag`/`±3`/`±-3`/`±4`/`±-4` families
for cubic). Symbol primes and the generator columns (`σ'(n)`) were treated only as secondary,
non-authoritative cross-checks, per the rationale that generators may not be 100% correct. For every
row, `unprime(M_derived)` was confirmed to reconstruct G's full Table 3 operation multiset exactly
(|M|=|G|), and the existing "Symmetry operators" entry was compared to `M_derived`:

- Tri/Mono/Ortho (12 rows: 23,25,27,29,30,31,33,35,36,38,39,40): all already matched the derivation
  exactly, including the bracketed/rotated-axis row 36 (`2'm'm`), which is internally self-consistent
  under M = H ∪ (G\H)' with H = `m`. No changes.
- Tetragonal (17 rows): two content errors fixed — `4'mm'` (row 53) and `4m'm'` (row 54) both had
  `2'_xy` where `-2'_xy` is required (4mm/C4v has only diagonal mirrors, no diagonal 2-folds, the same
  issue fixed for the unprimed `4mm` row in pass 2); `4/m'mm` (row 63) had `2_xy`/`-2'_xy` with the roles
  of the `xy`-diagonal mirror and 2-fold swapped between the H-part and the (G\H)'-part — fixed to
  `-2_xy` (H-part, matching `4mm`'s Table 3 ops) and `2'_xy` ((G\H)'-part). The other 14 rows
  (including the bracketed row 57, `-4'm2'`) already matched.
- Trigonal (6 rows: 67,69,71,73,74,75): row 67 already matched; rows 69, 71, 73, 74, 75 updated
  `n(m)`/`-n(m)` (prefix-minus, no `⊥`) to `n(m⊥)`/`n(-m⊥)` (infix-minus with `⊥`), matching Table 3's
  finalized trigonal notation — content unchanged.
- Hexagonal (17 rows): rows 77, 79, 81, 82, 83 already matched. Rows 85, 86, 88, 89, 92, 93, 95, 96,
  97, 98 updated `n(m)`/`-n(m)` groupings to `n(m⊥)`/`n(-m⊥)` (notation only, including the
  `6(2⊥)`↔`3(2⊥)`/`6(-2⊥)`↔`3(-2⊥)` family-count splitting for the `6/mmm`-derived rows). Rows 91
  (`-6'2m'`, the bracketed/rotated-axis special case) and 99 (`6'/mm'm`) additionally had `±6_z` and
  `±-6_z` swapped between the H-part and (G\H)'-part — fixed so that H (`32`/`-6m2`) carries
  `±3_z`/`±-6_z` as in Table 3's `-6m2`, and the (G\H)' part carries `±-6'_z`/`±6'_z` accordingly (row
  91's notation fixes also bring it in line with pass 2's `-6m2` fixes, resolving its
  previously-noted axis-convention transcription).
- Cubic (6 rows: 102,104,106,108,109,110): row 104 (`4'32'`) already matched exactly, validating the
  method. Rows 102 (`m'3`), 108 (`m3m'`), 109 (`m'3m'`) needed only prefix-minus→infix-minus notation
  updates (e.g. `-3(2)`→`3(-2')`, `-4(±3)`→`4(±-3')`, `-9(2)`→`9(-2')`, `-3(±4)`→`3(±-4')`, etc.; see
  pass 4 below for the prime-placement convention). Row 106 (`-4'3m'`) needed the notation update plus
  the inherited `-43m`-type content fix `3(±4')`→`3(±-4')`. Row 110 (`m'3m`) needed both the inherited
  H-part content fix (`3(±4)`→`3(±-4)`) and an independent (G\H)'-part content fix
  (`-3(±4')`→`3(±4')`, proper C4 not S4), confirmed via the unprime-reconstructs-G sanity check.

All 58 BW rows now satisfy `unprime(Symmetry operators) == G's Table 3 operation multiset` with
`|M| = |G|`, and use Table 3's finalized notation conventions throughout.

**2026-06 pass 4 (prime placement in grouped `n(m)` terms)**: In the grouped-operation notation
`n(m...)`, `n` is a multiplicity count (how many equivalent axes/operations of type `m...` there
are), not an operation itself, so it cannot carry a time-reversal prime. Every primed grouped term
of the form `n'(m...)` was corrected to `n(m'...)`, placing the prime on the operation symbol itself
— immediately after its rotation-order digit, in the same position as in ungrouped terms like
`2'_z` or `±4'_z` — consistent across both the trigonal/hexagonal `n(m⊥)`-style and cubic
`n(m)`-style families. Affected rows (all in the trigonal/hexagonal/cubic BW set, 23 terms total):
69, 71, 73, 74, 75, 85, 86, 88, 89, 91, 92, 93, 95 (×2), 96 (×2), 97, 98, 99 (×2), 102 (×2), 104, 106,
108 (×4), 109 (×3), 110 (×4). No element sets changed — this was a pure notation correction, and the
`unprime(M) == G` sanity check from pass 3 continues to hold for all 58 rows.

**2026-07 pass 5 (book-scan verification of six disputed rows; operator + generator columns)**: A
three-way consistency audit (operator column vs. σ(N)/σ'(N) closure vs. the `birss-app`
implementation, all 90 rows, exact eq.-2.17 matrices) flagged six rows, which were then read from
fresh scans of the printed book pages. Fixes:
- `-4'm2'` (bracketed/rotated row): operator column had been transcribed in the wrong axis frame —
  `-2_xy, -2_-xy, 2'_x, 2'_y` → `-2_x, -2_y, 2'_xy, 2'_-xy`. The book's row has unitary H = `mm2`
  with axis-aligned mirrors and primed diagonal 2-folds (confirmed by the scan, by ITC Table
  1.5.2.3, and by the row's own σ(3), σ(4) / σ'(8), which close exactly to the corrected list).
  Origin of the error: the pass-3 derivation embedded H = `mm2` inside the standard `-42m` frame
  ({1, 2_z, -2_xy, -2_-xy}), but the book's row is set in the `-4m2` frame — precisely the
  bracketed-row trap.
- `6'22'`: two missing time-reversal primes — `2_z, ±6_z` → `2'_z, ±6'_z` (book prints both
  underlined; also forced by the row's own H = `32`, |H| = 6).
- `6'mm'`: additional generator `σ'(5)` → `σ'(3)` (book prints σ̲(3); σ'(5) = m'_z is impossible,
  C6v contains no m_z).
- `-6m'2'`: additional generator `σ'(2)` → `σ'(4)` (book prints σ̲(4); m'⊥y matches the row's
  frame).
- `6'/m'mm'`: additional generator `σ'(2)` → `σ'(3)` — here the transcription was faithful and the
  **book itself misprints** σ̲(2): 2'_y collides with the unprimed 2_y ∈ H = `-3m`, and closing the
  printed generators yields the grey group `-3m1'` rather than a type-III group. New book misprint,
  analogous to the two documented in `conventions-reference.md`.
- `6'/mm'm` (documentation only, no change): the book prints generators σ(2), σ(5), σ(6); the
  transcribed σ(4), σ(5), σ(6) is the correct reading. σ(2) = 2_y would place an unprimed 2-fold on
  y, contradicting the row's full HM `6'/m 2'/m 2/m'` (position 2 = primed 2-fold, unprimed mirror
  ⊥y → generator σ(4) = m⊥y). Same σ(2)↔σ(4) misprint pattern as Table 3's documented `-6m2` case.

After this pass, closing each row's σ(N)/σ'(N) generators reproduces its operator column exactly
for all 90 rows (verified computationally).

**2026-06-30 independent verification (trigonal block, no changes)**: An independent audit of the
11 trigonal rows (`3, -3, -3', 32, 32', 3m, 3m', -3m, -3m', -3'm', -3'm`) re-derived the six primed
rows' Symmetry operators via `M = H ∪ (G\H)'` (§12 of `conventions-reference.md`) from Table 3, and
additionally cross-checked the block against scans of the original source, R. R. Birss, *Proc. Phys.
Soc.* **79**, 946 (1962), Table 2(a). No errors found — all 11 rows are internally consistent and
match both the group-theoretic derivation and the original source. This confirms, independently of
the "2026-06 pass 3" derivation above (which covers the same rows), that the trigonal block needs no
correction.

## References

- **Classical 32 point groups**: See Table 3
- **Magnetic symmetry operator definition**: Birss Chapter 3, §2
- **Time-reversal symmetry**: Birss Chapter 3, equation (3.15a)-(3.16b)
