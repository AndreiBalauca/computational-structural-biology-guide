# 01 — Workflow Overview

## Purpose

Computational structural biology is usually a workflow, not a single software step.

The general aim is to move from a protein target to a structure, prepare it properly, choose a suitable method, and analyse the result carefully.

---

## General Workflow

```text
Protein target
      ↓
Structure search
      ↓
Structure quality check
      ↓
Molecular visualisation
      ↓
Protein / ligand preparation
      ↓
Docking, MD, or AI modelling
      ↓
Analysis
      ↓
Documentation
```

---

## Main Stages

| Stage | Main question |
|---|---|
| Target selection | What protein or system am I studying? |
| Structure search | Is there an experimental or predicted structure? |
| Quality check | Is the structure suitable to use? |
| Visualisation | What does the structure actually look like? |
| Preparation | Are the protein and ligand ready for computation? |
| Method choice | Should I use docking, MD, AI modelling, or another method? |
| Analysis | What does the output show? |
| Documentation | Could someone else repeat the workflow? |

---

## Why This Matters

A common beginner mistake is to download a structure and immediately run docking or MD.

A better approach is:

```text
download structure
      ↓
inspect it
      ↓
check missing regions, ligands, cofactors, and biological state
      ↓
prepare the system
      ↓
choose the method
      ↓
run calculation
      ↓
analyse carefully
```

Bad input structures usually lead to unreliable results.

---

## Choosing the Method

| Method | Useful for | Main caution |
|---|---|---|
| Visualisation | Checking structures and making figures | A nice-looking structure can still be unsuitable |
| Docking | Predicting possible ligand poses | Docking scores are not proof of binding |
| Molecular dynamics | Studying motion and stability over time | Short simulations should not be overinterpreted |
| AI structure prediction | Getting models when no structure exists | Confidence scores must be checked |
| Cheminformatics | Working with molecules and datasets | Data quality and standardisation matter |

---

## Basic Checks Before Computation

Before running docking, MD, or AI modelling, check:

- structure source
- experimental or predicted structure
- missing residues or atoms
- ligands, cofactors, ions, or waters
- biological assembly
- protein state or conformation
- whether the method matches the question

---

## Common Mistakes

- running software before checking the structure
- trusting docking scores without visual inspection
- treating AI models as experimental evidence
- ignoring missing residues or cofactors
- using the wrong biological assembly
- overinterpreting one short MD simulation
- not recording commands, software versions, or parameters

---

## Key Takeaway

A good computational workflow is careful, reproducible, and cautious. The aim is not just to produce an output, but to understand whether the output is reliable.
