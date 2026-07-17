# 06 — Molecular Docking

## Purpose

Molecular docking is used to predict possible binding poses between a ligand and a protein binding site.

It can help generate hypotheses about how a molecule may interact with a target.

---

## Basic Docking Workflow

```text
prepare protein
      ↓
prepare ligand
      ↓
define binding site
      ↓
run docking
      ↓
inspect poses
      ↓
compare interactions
```

---

## What Docking Can Show

Docking can suggest:

- possible ligand binding poses
- important residues near the ligand
- hydrogen bonds
- hydrophobic contacts
- salt bridges
- steric clashes
- rough pose ranking

---

## What Docking Cannot Prove

Docking does not prove:

- that a ligand truly binds
- the real binding free energy
- biological activity
- receptor activation or inhibition
- that the top-scoring pose is correct

Docking results should be treated as hypotheses.

---

## Common Tools

| Tool | Use |
|---|---|
| AutoDock Vina | Open-source molecular docking |
| GNINA | Docking with machine-learning scoring |
| Glide | Commercial docking software |
| PyMOL / ChimeraX | Visual inspection of poses |
| Open Babel | Ligand format conversion |

---

## Important Checks

Before trusting docking results, check:

- protein preparation
- ligand protonation state
- ligand stereochemistry
- binding site location
- grid box placement
- whether cofactors, ions, or waters are important
- whether the pose makes chemical sense

---

## Common Mistakes

- trusting docking score alone
- not checking poses visually
- docking into the wrong binding site
- using the wrong protonation state
- ignoring important waters, ions, or cofactors
- assuming docking proves binding
- comparing scores across very different systems too strongly

---

## Key Takeaway

Docking is useful for generating binding hypotheses, but the results need visual inspection, chemical reasoning, and further validation.
