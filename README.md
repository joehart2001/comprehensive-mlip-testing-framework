# A Comprehensive Testing Suite for Foundation MLIPs

This repository provides a comprehensive testing framework and interactive analysis suite for foundation Machine Learning Interatomic Potentials (MLIPs). The interactive analysis suite is currently hosted at:
[http://mlip-testing.stfc.ac.uk:8050](http://mlip-testing.stfc.ac.uk:8050)

Key goals of this framework include:
- Testing physics: Moving away from benchmarking solely on energies and forces
    - MD tests, NEBs, phonons, elastic moduli, and more
- Breadth: Testing on a wide range of systems to truly assess the ability of foundation MLIPs
    - Bulk inorganic crystals, molecular crystals, molecules, surfaces, MOFs, supramolecular systems, and more
- Depth: the ability to swiftly investigate numbers, outliers and trends through an interactive analysis suite featuring:
    - Interactive tables
    - Interactive plots
    - Structural visualisation
    - Custom benchmark weights


### Summary of currently implemented tests:
<p align="center">
  <img src="docs/images/benchmark_summary.png" alt="Benchmark Summary" width="900">
</p>




## Benchmark & Test Coverage

Below is an overview of current and planned benchmarks, including whether each is implemented in the suite, whether a script is available, and whether reference data exists.

### Legend
- ✅ = Yes / Implemented
- ❌ = No / Not yet
- ⬜ = Planned

---

## MACE-MP-0 Tests

| Test Name | Category | Script Ready? | Implemented? | Level of Theory |
|-----------|----------|---------------|--------------|-----------------|
| A.1 Self-interstitials in silicon | Bulk Defects | ❌ | ❌ |  |
| A.2 Amorphous silicon from melt–quench | Amorphous | ❌ | ❌ |  |
| A.3 Amorphous carbon | Amorphous | ❌ | ❌ |  |
| A.4 Ceria nanoparticles | Nanoparticles | ❌ | ❌ |  |
| A.5 Inorganic halide perovskite | Perovskites | ❌ | ❌ |  |
| A.6 Hybrid Organic–Inorganic Perovskites (HOIPs) | Perovskites | ❌ | ❌ |  |
| A.7 Protein dynamics & stability | Biomolecules | ❌ | ❌ |  |
| A.8 Hydrogen combustion | Reactions / MD | ❌ | ❌ |  |
| A.9 Sulfur polymerisation | Polymers | ❌ | ❌ |  |
| A.10 Zeolites | Porous materials | ❌ | ❌ |  |
| A.11 Open-circuit voltage of lithiated graphite | Batteries | ❌ | ❌ |  |
| A.12 Jahn–Teller distortions in LiNiO₂ | Transition Metal Oxides | ❌ | ❌ |  |
| A.13 Point & extended defects in BCC metals | Bulk Defects | ❌ | ❌ |  |
| A.14 Alumina defects & bulk diffusion | Oxides | ❌ | ❌ |  |
| A.15 Random structure search: Arsenic | Structure Search | ❌ | ❌ |  |
| A.16 Properties of bulk & nanoconfined water | Liquids | ❌ | ❌ |  |
| A.17 Ethanol–water density–composition curves | Liquids | ❌ | ❌ |  |
| A.18 Solvent mixtures | Liquids | ❌ | ❌ |  |
| A.19 Aqueous interfaces | Interfaces | ❌ | ❌ |  |
| A.20 Molten salts | Liquids | ❌ | ❌ |  |
| A.21 Room-temperature ionic liquids | Liquids | ❌ | ❌ |  |
| A.22 High-pressure hydrogen | High-Pressure | ❌ | ❌ |  |
| A.23 Ammonia & borane thermal decomposition | Reactions | ❌ | ❌ |  |
| A.24 Heterogeneous catalysis | Surfaces / Catalysis | ❌ | ❌ |  |
| A.25 Carborane rearrangement | Reactions | ❌ | ❌ |  |
| A.26 Transition metal dichalcogenides | 2D Materials | ❌ | ❌ |  |
| A.27 Electrode–electrolyte interface / Battery system | Batteries | ❌ | ❌ |  |
| A.28 Metal–organic frameworks (MOFs) | Porous Materials | ❌ | ❌ |  |
| A.29 Combinatorial materials discovery | Materials Discovery | ❌ | ❌ |  |
| A.30 Alanine tripeptide free energy surface | Biomolecules | ❌ | ❌ |  |
| A.31 Molecule–surface interactions | Surfaces | ❌ | ❌ |  |
| A.32 Computational efficiency (twenty-element alloy) | Performance | ❌ | ❌ |  |
| A.33 MPA-0: Scaling up with the Alexandria dataset | Dataset Scaling | ❌ | ❌ |  |


## MACE-MP-0 Benchmarks

| Test Name | Category | Script Ready? | Implemented? | Level of Theory |
|-----------|----------|---------------|--------------|-----------------|
| B.1 Phonons | Bulk Crystals | ❌ | ❌ |  |
| B.2 Bulk & shear moduli | Bulk Crystals | ❌ | ❌ |  |
| B.3 Cohesive energies | Bulk / Molecular Crystals | ❌ | ❌ |  |
| B.4 Atomization energies & lattice constants of solids | Bulk Crystals | ❌ | ❌ |  |
| B.5 Reaction barrier heights | Molecules | ❌ | ❌ |  |
| B.6 Homonuclear diatomics | Molecules | ❌ | ❌ |  |


---

### Planned Additional Benchmarks

| Test Name | Category | Script Ready? | Implemented? | Level of Theory |
|-----------|----------|---------------|--------------|-----------------|
| EOS metals (various sizes) | Bulk Crystals | ❌ | ❌ | PBE |
| Thermal conductivity | Bulk Crystals | ❌ | ❌ | PBE |
| Formation energies | Bulk Crystals | ❌ | ❌ | PBE / Experiment |
| Dimer interactions (S66) | Molecular | ❌ | ❌ | CCSD(T) |
| GMTKN55 (5 categories) | Molecules | ❌ | ❌ | Various high-level |
| O₂ / H₂ reaction profiles | Molecules | ❌ | ❌ | PBE |
| Torsion curves | Molecules | ❌ | ❌ | CCSD(T) / PBE |
| X24 (molecule–surface) | Surfaces | ❌ | ❌ | PBE |
| OC20 | Surfaces | ❌ | ❌ | PBE |
| QMOF | MOFs | ❌ | ❌ | PBE |
| RDF/density of liquids | Liquids | ❌ | ❌ | Experiment / DFT |


---

## Electrostatic Paper Benchmarks

### Main group thermo-chemistry
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| GMTKN55 | ❌ | ✅ | Various high-level |
| MB2061 Mindless molecules | ❌ | ✅ |  |
| BH9 reactions | ❌ | ✅ |  |


### Non-covalent interactions
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| NCIA IHB100x10: benchmark of h-bonds involving ions | ❌ | ✅ |  |
| NCIA HB375x10: benchmark of h-bonds | ❌ | ✅ |  |
| NCIA HB300SPX: H bonds involving S, P, halogens | ❌ | ✅ |  |
| NCIA D1200 London dispersion | ❌ | ✅ |  |
| NCIA D442x10 London dispersion dissociation curves | ❌ | ✅ |  |
| NCIA SH250x10 sigma-hole interactions (halogen/chalcogen/pnictogen bonds) | ❌ | ✅ |  |
| NCIA R739x5 repulsive contacts | ❌ | ✅ |  |
| S30L | ❌ | ✅ |  |
| PLA15 for protein fragments interaction energies | ❌ | ✅ |  |
| PLF547 for dimers interactions | ❌ | ✅ |  |
| IONPI19 molecule-ion pairs | ❌ | ✅ |  |


### Conformer Energies
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| 37CONF8 | ❌ | ✅ |  |
| ACONFL | ❌ | ✅ |  |
| DipConfs | ❌ | ✅ |  |
| Glucose205 | ❌ | ✅ |  |
| Maltose222 | ❌ | ✅ |  |
| MPCONF196 | ❌ | ✅ |  |
| OpenFF-Tors | ❌ | ✅ |  |
| TMCONF16 | ❌ | ✅ |  |
| UPU46 | ❌ | ✅ |  |


### Transition metals
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| 3dmtv | ❌ | ✅ |  |
| mme55 | ❌ | ✅ |  |
| mor41 | ❌ | ✅ |  |
| rot61 | ❌ | ✅ |  |


### Barrier heights
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| BH2O-36 hydrolysis barrier heights | ❌ | ✅ |  |
| Proton, hydride, CH₃ migration reactions in carbocations | ❌ | ✅ |  |
| Barriers and reaction energies in a multi-step reaction chain | ❌ | ✅ |  |
| Pericyclic reactions | ❌ | ✅ |  |
| PX13 Proton exchange barriers for H₂O, NH₃ and HF clusters (inside GMTKN55) | ❌ | ✅ |  |


### Others
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| Mindless molecules | ❌ | ✅ |  |
| Minnesota database | ❌ | ✅ |  |
| CARBO33 carbocation relative energies and some reactions involving bigger systems | ❌ | ✅ |  |






