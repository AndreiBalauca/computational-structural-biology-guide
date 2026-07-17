# 11 — Analysis and Interpretation

## Purpose

Computational results need to be analysed carefully before making conclusions.

The output from docking, MD, or AI modelling is only useful if it is checked and interpreted properly.

---

## Common Analysis Types

| Analysis | Use |
|---|---|
| Visual inspection | Checks whether results make structural sense |
| RMSD | Measures overall structural change |
| RMSF | Measures residue flexibility |
| Distances | Tracks separation between atoms or residues |
| Hydrogen bonds | Checks specific interactions |
| Contacts | Identifies nearby residues or ligand interactions |
| Clustering | Groups similar conformations or poses |
| Energy or score comparison | Helps rank results, but should be used cautiously |

---

## Docking Analysis

Docking results should be checked for:

- binding pose
- docking score
- hydrogen bonds
- hydrophobic contacts
- salt bridges
- steric clashes
- whether the pose fits the known biology

The best score is not always the best pose.

---

## MD Analysis

MD trajectories can be checked for:

- system stability
- protein movement
- ligand stability
- residue flexibility
- important distances
- hydrogen bonds over time
- changes in binding-site shape

For more detailed AMBER trajectory analysis notes, see the analysis section in my separate `amber-md-notes` repository.

A short trajectory can show setup problems, but it should not be overinterpreted.

---

## AI Model Interpretation

AI-predicted structures should be checked for:

- confidence scores
- low-confidence regions
- missing ligands or cofactors
- biological relevance
- agreement with experimental structures, if available

A confident-looking model is not automatically correct.

---

## Common Mistakes

- relying on one score or one plot
- ignoring visual inspection
- overinterpreting short MD simulations
- treating docking scores as binding free energies
- treating AI models as experimental evidence
- not checking whether the result matches the biological question
- making strong claims without enough validation

---

## Key Takeaway

Good analysis combines numbers, visual inspection, chemical reasoning, and biological context. Results should be interpreted cautiously, especially from docking, short MD runs, or predicted structures.
