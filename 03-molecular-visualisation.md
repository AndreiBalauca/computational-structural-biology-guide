# 03 — Molecular Visualisation

## Purpose

Molecular visualisation is used to inspect protein structures before running docking, molecular dynamics, or other computational methods.

It helps check whether a structure is complete, biologically relevant, and suitable for further work.

---

## Common Tools

| Tool | Main use |
|---|---|
| PyMOL | Protein structure inspection and figure making |
| ChimeraX | Structure visualisation, analysis, and model inspection |
| VMD | Molecular dynamics trajectory visualisation |
| NGL Viewer | Quick browser-based structure viewing |

---

## What to Check

When opening a structure, check:

- protein chains
- ligands
- binding site
- missing residues
- cofactors or ions
- waters
- mutations
- unusual clashes or geometry
- membrane position, if relevant

---

## Example Visualisation Workflow

```text
open structure
      ↓
identify chains
      ↓
show ligand or binding site
      ↓
check missing regions
      ↓
inspect important residues
      ↓
save notes or figures
```

---

## Why Visualisation Matters

A structure may look usable from a database page, but problems are often easier to notice visually.

For example:

- the ligand may not be in the expected binding site
- part of the protein may be missing
- the structure may contain engineered mutations
- waters, ions, or cofactors may be important
- the biological assembly may differ from the downloaded chain

---

## Common Representations

| Representation | Use |
|---|---|
| Cartoon | Overall protein fold |
| Sticks | Ligands and side chains |
| Surface | Binding pockets and shape |
| Spheres | Ions or selected atoms |
| Lines | Waters or less important atoms |

---

## Common Mistakes

- using a structure without visually inspecting it
- only looking at the whole protein and ignoring the binding site
- hiding ligands, ions, or cofactors by accident
- making figures before understanding the structure
- assuming a nice-looking image means the structure is suitable
- not checking missing loops or residues

---

## Key Takeaway

Molecular visualisation is a quality-control step. Before running calculations, the structure should be inspected carefully, especially the chains, ligands, binding site, missing regions, and biologically important features.
