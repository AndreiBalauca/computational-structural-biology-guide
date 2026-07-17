# 04 — Molecular File Formats

## Purpose

Different molecular file formats store different types of information.

Some store sequences, some store 3D coordinates, some store chemical information, and some store simulation data.

---

## Common File Formats

| Format | Main use |
|---|---|
| FASTA | Protein or DNA/RNA sequence |
| PDB | 3D protein or complex structure |
| mmCIF | Modern format for structural biology data |
| MOL2 | Small-molecule structure with atom types |
| SDF | Small-molecule data and properties |
| SMILES | Text form of a molecule |
| PDBQT | AutoDock Vina docking format |
| PRMTOP | AMBER topology file |
| INPCRD / RST | AMBER coordinate or restart file |
| NC | AMBER trajectory file |
| GRO | GROMACS structure file |
| TOP | GROMACS topology file |
| XTC | GROMACS trajectory file |

---

## Key Difference

A structure file and a topology file are not the same thing.

| File type | Contains |
|---|---|
| Structure file | Atom positions |
| Topology file | Atom types, bonds, charges, and force field information |
| Trajectory file | Movement over time |

For example, an MD trajectory usually needs a matching topology or structure file to be analysed properly.

---

## Examples

| Task | Possible file formats |
|---|---|
| View a protein | PDB or mmCIF |
| Store a sequence | FASTA |
| Prepare a ligand | SDF, MOL2, or SMILES |
| Run docking | PDBQT |
| Run AMBER MD | PRMTOP + INPCRD/RST |
| Run GROMACS MD | GRO + TOP |
| Analyse a trajectory | NC or XTC with topology |

---

## Common Mistakes

- renaming a file instead of converting it properly
- assuming PDB files contain reliable charges
- treating SMILES as a 3D structure
- using a trajectory without the correct topology
- confusing AMBER and GROMACS file types
- assuming conversion keeps all chemical information

---

## Key Takeaway

File formats matter because they control what information is stored. Before using or converting a file, check whether it contains the coordinates, topology, charges, bonds, and chemical information needed for the task.
