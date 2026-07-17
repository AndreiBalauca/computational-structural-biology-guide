# 07 — AMBER Workflow Overview

## Purpose

AMBER is used for molecular dynamics simulations, especially for proteins, nucleic acids, ligands, and biomolecular complexes.

This file gives a broad overview. For more detailed AMBER notes, see my separate `amber-md-notes` repository.

---

## Basic AMBER Workflow

```text
prepare structure
      ↓
build topology and coordinates
      ↓
minimise system
      ↓
heat system
      ↓
equilibrate system
      ↓
run production MD
      ↓
analyse trajectory
```

---

## Main Files

| File | Use |
|---|---|
| `.pdb` | Starting structure |
| `.prmtop` | AMBER topology file |
| `.inpcrd` | AMBER coordinate file |
| `.in` | Simulation input file |
| `.rst` | Restart file |
| `.out` | Output log file |
| `.mdinfo` | Short progress/status file |
| `.nc` | Trajectory file |

---

## Main Programs

| Program | Use |
|---|---|
| `pdb4amber` | Cleans PDB files for AMBER |
| `tleap` | Builds topology and coordinate files |
| `sander` | Runs minimisation and MD |
| `pmemd` | Faster MD engine, often used for production |
| `cpptraj` | Trajectory analysis |

---

## Typical Simulation Stages

| Stage | Purpose |
|---|---|
| Minimisation | Removes bad contacts and relaxes geometry |
| Heating | Raises the system to the target temperature |
| Equilibration | Allows the system to stabilise |
| Production MD | Generates the trajectory used for analysis |
| Trajectory analysis | Measures movement, stability, contacts, and interactions |

---

## Common Analysis Outputs

AMBER trajectories can be analysed for:

- RMSD
- RMSF
- distances
- hydrogen bonds
- contacts
- clustering
- radius of gyration
- visual trajectory inspection

---

## Common Mistakes

- using the wrong topology file
- forgetting that trajectories need the matching topology
- skipping minimisation or equilibration
- overinterpreting short simulations
- not checking output files
- not recording input parameters
- uploading research trajectories or unpublished data publicly

---

## Key Takeaway

AMBER is a full molecular dynamics workflow, not just one command. The topology, coordinates, input files, simulation stages, and trajectory analysis all need to match and be documented carefully.
