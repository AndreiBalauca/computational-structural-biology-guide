# Common Mistakes

## Purpose

This file summarises common beginner mistakes in computational structural biology workflows.

Most problems come from using software before checking the structure, inputs, or scientific question.

---

## Structure Selection

Common mistakes:

- choosing the first structure found
- not checking experimental method or resolution
- ignoring missing residues or atoms
- not checking ligands, cofactors, ions, or waters
- using the wrong biological assembly
- treating AI-predicted structures like experimental structures

---

## Visualisation

Common mistakes:

- not opening the structure before using it
- only looking at the whole protein
- ignoring the binding site
- hiding ligands or cofactors by accident
- making figures before understanding the structure

---

## File Formats

Common mistakes:

- renaming files instead of converting them properly
- confusing structure files with topology files
- using trajectories without the correct topology
- assuming PDB files contain full chemical information
- mixing AMBER and GROMACS file types

---

## Protein and Ligand Preparation

Common mistakes:

- deleting important ions, waters, or cofactors
- ignoring protonation states
- using the wrong ligand stereochemistry
- not checking missing residues
- assuming database structures are ready to use directly

---

## Docking

Common mistakes:

- trusting docking scores alone
- not inspecting poses visually
- docking into the wrong site
- using the wrong ligand state
- treating docking as proof of binding

---

## Molecular Dynamics

Common mistakes:

- skipping minimisation or equilibration
- using the wrong topology file
- not checking output files
- overinterpreting short simulations
- not recording input parameters
- not keeping track of software versions

---

## AI-Predicted Structures

Common mistakes:

- ignoring confidence scores
- docking into low-confidence regions
- using predicted structures without checking related experimental structures
- overclaiming from one model
- forgetting ligands, cofactors, ions, and waters may be missing

---

## Public Repository Safety

Do not upload:

- unpublished research structures
- lab-owned files
- confidential scripts
- trajectories from active projects
- docking results from unpublished work
- project-specific figures or analysis without permission

Use public repositories for:

- generic notes
- public examples
- learning workflows
- command explanations
- reproducible documentation practice

---

## Key Takeaway

Most mistakes are avoidable by checking the structure, file formats, preparation steps, method choice, and outputs before making conclusions.
