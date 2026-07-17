# 10 — AI-Predicted Structures

## Purpose

AI-predicted structures can be useful when no experimental structure is available.

They should be treated as structural hypotheses, not the same as experimental evidence.

---

## Common Sources and Tools

| Tool / database | Use |
|---|---|
| AlphaFold DB | Predicted protein structures |
| AlphaFold Server | Protein and complex structure prediction |
| Boltz | Biomolecular structure prediction |
| Chai-1 | Structure prediction for biomolecular systems |
| Protenix | AI-based biomolecular modelling |

---

## When AI Structures Are Useful

AI-predicted structures can help when:

- no experimental structure exists
- only a related protein has a structure
- a starting model is needed
- comparing possible domains or folds
- planning docking or MD carefully

---

## What to Check

Before using an AI-predicted structure, check:

- confidence scores
- low-confidence regions
- missing ligands, cofactors, ions, or waters
- whether the model represents the correct biological state
- whether the binding site is reliable
- whether experimental structures of related proteins exist

---

## Main Caution

AI models can look very convincing visually.

However, they may still be unreliable in:

- flexible loops
- disordered regions
- binding sites
- ligand-bound states
- membrane orientation
- protein complexes
- active vs inactive conformations

---

## Common Mistakes

- treating predicted structures as experimental structures
- ignoring confidence scores
- docking into low-confidence regions
- using predicted binding sites without checking evidence
- forgetting that ligands, cofactors, and waters may be absent
- overclaiming based on one predicted model

---

## Key Takeaway

AI-predicted structures are useful starting points, but they must be checked carefully before docking, molecular dynamics, or biological interpretation.
