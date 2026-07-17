# 02 — Finding Protein Structures

## Purpose

The first practical step in many computational structural biology projects is finding a suitable structure for the protein or complex being studied.

A structure may come from experimental methods such as X-ray crystallography, cryo-EM, or NMR, or from prediction methods such as AlphaFold.

---

## Main Structure Sources

| Resource | Use |
|---|---|
| RCSB PDB | Experimental protein, nucleic acid, and complex structures |
| AlphaFold DB | Predicted protein structures |
| UniProt | Protein sequence, function, domains, and variants |
| GPCRdb | GPCR structures, residue numbering, and diagrams |
| PubMed | Papers describing structures, ligands, mutations, or mechanisms |

---

## Experimental vs Predicted Structures

| Structure type | Useful for | Main caution |
|---|---|---|
| X-ray crystallography | High-resolution atomic detail | May contain missing flexible regions or crystal artefacts |
| Cryo-EM | Large complexes and membrane proteins | Local resolution can vary |
| NMR | Solution-state structural ensembles | Usually smaller systems |
| AlphaFold / AI-predicted | When no experimental structure exists | Confidence scores and biological relevance must be checked |

---

## Basic Search Workflow

```text
protein name
      ↓
UniProt entry
      ↓
RCSB PDB search
      ↓
AlphaFold DB if no suitable experimental structure exists
      ↓
read linked paper
      ↓
inspect structure visually
```

---

## What to Record

For each structure, record:

- PDB ID or AlphaFold ID
- protein name
- organism
- experimental method or prediction method
- resolution, if experimental
- chain used
- ligands, cofactors, ions, or waters
- missing residues or mutations
- linked paper or database source

---

## Common Mistakes

- choosing the first structure found without checking quality
- ignoring whether the structure is active, inactive, apo, or ligand-bound
- missing important ligands, ions, cofactors, or waters
- using an engineered construct without noticing
- treating an AlphaFold model as equivalent to an experimental structure
- not reading the paper linked to the structure

---

## Key Takeaway

Finding a structure is not just downloading a file. The structure must be checked for source, quality, biological relevance, missing regions, and suitability for the planned method.
