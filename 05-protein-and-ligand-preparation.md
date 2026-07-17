# 05 — Protein and Ligand Preparation

## Purpose

Before docking or molecular dynamics, protein and ligand structures need to be prepared.

Raw structures from databases are often not ready to use directly.

---

## Protein Preparation

Protein preparation may include:

- choosing the correct chain
- removing unwanted molecules
- checking missing residues or atoms
- adding hydrogens
- assigning protonation states
- keeping important ligands, ions, cofactors, or waters
- checking residue names
- preparing the structure for a specific software package

---

## Ligand Preparation

Ligand preparation may include:

- checking the correct chemical structure
- adding hydrogens
- assigning protonation state
- generating 3D coordinates
- checking stereochemistry
- minimising the ligand
- converting to the required file format

---

## Important Decisions

| Decision | Why it matters |
|---|---|
| Keep or remove waters | Some waters may be important for binding |
| Keep or remove ions | Ions can stabilise structures or binding sites |
| Protonation state | Affects charge and interactions |
| Ligand stereochemistry | Wrong stereochemistry can change binding |
| Missing residues | May affect binding sites or stability |
| Chain selection | The downloaded structure may contain multiple chains |

---

## Common Tools

| Tool | Use |
|---|---|
| PyMOL / ChimeraX | Visual inspection and simple editing |
| pdb4amber | Preparing PDB files for AMBER |
| tleap | Building AMBER topology and coordinate files |
| Open Babel | File conversion and ligand handling |
| RDKit | Ligand handling and cheminformatics |
| CHARMM-GUI | System building, especially membrane systems |

For more detailed AMBER-specific notes, see my separate `amber-md-notes` repository.

---

## Common Mistakes

- deleting important cofactors or ions
- ignoring protonation states
- using the wrong ligand structure
- forgetting stereochemistry
- assuming the downloaded PDB is ready to use
- removing waters without checking if they are important
- not checking the structure visually after preparation

---

## Key Takeaway

Preparation is one of the most important steps. A docking or MD result is only useful if the protein and ligand were prepared correctly.
