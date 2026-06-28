# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

This repository contains digitized final exam papers for the Solid State Physics (固体物理) course at Nanjing University, spanning **2004 through 2017**. All content is transcribed from original handwritten/printed exam papers into Markdown with inline LaTeX math.

This is a **pure document repository** — there is no build system, no code, and no automated tests.

## File naming convention

Exam files follow the pattern:

```
{year}[_-]{optional-semester}_固体物理期末[_instructor].md
```

Examples:
- `2017_固体物理期末.md` — 2017 exam, no instructor/semester in filename
- `2016-2017_固体物理期末.md` — academic year 2016–2017 (first semester)
- `2004_固体物理期末_胡安.md` — 2004 exam by instructor 胡安 (with 章维益)
- `2013期末_Word版.md` — alternate 2013 exam version, different naming convention

The `README.md` contains a brief description of the transcription project.

## Formatting conventions

- **Math formulas**: Inline math uses `$...$`, display math uses `$$...$$`. All are standard LaTeX syntax.
- **Illegible content**: Marked as `【不清晰】` (Chinese for "unclear"). Used when the original handwritten text is ambiguous or obscured by corrections. Some files also include inline notes like `【该问后半句字迹较模糊】` explaining the uncertainty.
- **File structure**: Each exam file starts with a level-1 heading (`#`) with the year and course name, followed by a blockquote note if there are transcription caveats. Each major problem is a level-2 heading (`##`) labeled with Chinese numbering (一、二、三、四). Sub-problems use numbered lists. Teacher names and semester info, when known, appear in the heading or first paragraph.
- **Physical constants**: Some exams include formula sheets or constant references inline; notation varies slightly across years but follows standard solid-state physics conventions (e.g., `E_F^0` for Fermi energy at T=0, `Ω_BZ` for Brillouin zone volume).

## Topic coverage

The exams cover the standard NJU Solid State Physics curriculum. Recurring topics across the collection:

- **Crystal structure**: Bravais lattices, point groups (点群) and space groups (空间群), primitive vs. conventional cells, Miller indices and interplanar spacing, geometric structure factors and extinction conditions (bcc, fcc, sc, diamond, CsCl, Cu₂O)
- **Lattice dynamics**: Monatomic chain dispersion, Einstein model, Debye model (density of states, zero-point energy, Debye temperature, low-temperature phonon number, heat capacity); phonon branch counting (LO/TO/LA/TA modes for given crystal structures)
- **Crystal binding**: Madelung energy, Born-Mayer repulsion (NaCl), interatomic potentials and elastic constants, cohesive energy
- **Electronic band theory**: Nearly-free electron approximation (periodic potential, band gaps at BZ boundaries, wavefunctions), tight-binding approximation (s-orbitals on sc, orthorhombic, tetragonal lattices; E(k) formulas, effective mass tensor, DOS), Wannier functions (orthogonality proof, localization); two-band model for semiconductors (semiclassical dynamics with conduction/valence bands)
- **Low-dimensional systems**: 2D free electron gas (density of states, finite-T chemical potential), 2D Bravais lattices and Wigner-Seitz cells (graphene as a 2D composite lattice)
- **Free electron gas**: Fermi energy/wavevector, density of states, average energy per electron, electronic specific heat, Pauli paramagnetism; electron-hole formalism (hole k, energy, effective mass, velocity, equations of motion)
- **Collective excitations**: Plasmons (plasmon frequency, dependence on electron density), electron correlation and screening
- **Semiclassical dynamics**: Equations of motion under external E/B fields (k-evolution, cyclotron frequency); Boltzmann equation in relaxation-time approximation
- **Transport**: Temperature dependence of resistivity (electron-phonon scattering: ρ ∝ T⁵ at low T, ρ ∝ T at high T); Peierls transition
- **X-ray diffraction**: Bragg's law, powder diffraction patterns, extinction rules
- **Thermal properties**: Thermal expansion (zero in harmonic approximation), specific heat (electronic + phonon contributions)

## Adding new exams

When transcribing a new exam paper:

1. Name the file following the existing pattern: `{year}[_-]{semester}_固体物理期末[_instructor].md`
2. Start with a level-1 heading: `# {year} 固体物理期末原题`
3. Add a blockquote note if any parts are unclear or the source is handwritten
4. Structure problems as level-2 headings with Chinese numbering (`## 一、...`, `## 二、...`, etc.)
5. Use `$...$` for inline math and `$$...$$` for display/block math
6. Mark any illegible or ambiguous content with `【不清晰】`
7. Keep instructor names and semester info (A卷/B卷, time limit) in the opening text when available
