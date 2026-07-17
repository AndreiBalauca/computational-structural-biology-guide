# 08 — GROMACS Workflow Overview

## Purpose

GROMACS is a molecular dynamics package used to simulate proteins, membranes, ligands, and other biomolecular systems.

This file gives a short overview of the main workflow and file types.

---

## Basic GROMACS Workflow

```text
prepare structure
      ↓
generate topology
      ↓
define simulation box
      ↓
solvate system
      ↓
add ions
      ↓
minimise system
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
| `.gro` | GROMACS structure file |
| `.top` | Topology file |
| `.itp` | Included topology file |
| `.mdp` | Simulation parameter file |
| `.tpr` | Portable run input file |
| `.xtc` | Compressed trajectory file |
| `.trr` | Full-precision trajectory file |
| `.edr` | Energy file |
| `.log` | Simulation log file |

---

## Main Programs

| Command | Use |
|---|---|
| `pdb2gmx` | Generates topology from a structure |
| `editconf` | Defines box and edits coordinates |
| `solvate` | Adds solvent |
| `grompp` | Prepares the run input file |
| `mdrun` | Runs the simulation |
| `trjconv` | Processes trajectories |
| `rms`, `rmsf`, `hbond` | Common analysis tools |

---

## Typical Simulation Stages

| Stage | Purpose |
|---|---|
| Energy minimisation | Removes bad contacts |
| NVT equilibration | Stabilises temperature |
| NPT equilibration | Stabilises pressure and density |
| Production MD | Generates the trajectory for analysis |
| Analysis | Measures stability, motion, and interactions |

---

## AMBER vs GROMACS

| AMBER | GROMACS |
|---|---|
| Uses `.prmtop` and `.inpcrd` | Uses `.top`, `.gro`, and `.tpr` |
| Common in AMBER force field workflows | Very common for large-scale MD |
| Uses `sander`, `pmemd`, `cpptraj` | Uses `grompp`, `mdrun`, and GROMACS analysis tools |

Both can be used for molecular dynamics. The best choice depends on the system, force field, lab workflow, and available computing resources.

---

## Common Mistakes

- confusing `.gro`, `.top`, and `.tpr` files
- skipping equilibration
- using the wrong force field
- ignoring warnings from `grompp`
- analysing a trajectory without the correct structure or topology
- overinterpreting one short simulation
- not recording `.mdp` parameters

---

## Key Takeaway

GROMACS is another major MD workflow. Like AMBER, it depends on correct preparation, topology generation, equilibration, production MD, and careful trajectory analysis.
