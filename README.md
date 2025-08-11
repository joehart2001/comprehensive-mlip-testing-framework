# A Comprehensive Testing Suite for Foundation MLIPs

This repository provides a comprehensive testing framework and interactive analysis suite for foundation Machine Learning Interatomic Potentials (MLIPs). The interactive analysis suite is currently hosted at:
[http://mlip-testing.stfc.ac.uk:8050](http://mlip-testing.stfc.ac.uk:8050)

Key features of this framework include:
- Testing physics: Moving away from benchmarking solely on energies and forces
    - MD tests, NEBs, phonons, elastic moduli, and more
- Breadth: Testing on a wide range of systems to truly assess the ability of foundation MLIPs
    - Bulk inorganic crystals, molecular crystals, molecules, surfaces, MOFs, supramolecular systems, and more
- Depth: the ability to swiftly investigate numbers, outliers and trends through an interactive analysis suite featuring: interactive tables, interactive plots, structural visualisation and custom benchmark weights

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


## MACE-MP-0 Benchmarks

| Test Name | Category | Script Ready? | Implemented? | Level of Theory |
|-----------|----------|---------------|--------------|-----------------|
| B.1 Phonons | Bulk Crystals | ✅ | ✅ | PBE |
| B.2 Bulk & shear moduli | Bulk Crystals | ✅ | ✅ | PBE |
| B.3 Cohesive energies | Bulk / Molecular Crystals | ✅ | ✅ | DMC/PBE |
| B.4 Atomization energies & lattice constants of solids | Bulk Crystals | ❌ | ❌ |  |
| B.5 Reaction barrier heights | Molecules | ❌ | ❌ |  |
| B.6 Homonuclear diatomics | Molecules | ✅ | ✅ | N/A |


---

## Planned Additional Benchmarks

| Test Name | Category | Script Ready? | Implemented? | Level of Theory |
|-----------|----------|---------------|--------------|-----------------|
| EOS metals (various sizes) | Bulk Crystals | ❌ | ❌ |  |
| Thermal conductivity | Bulk Crystals | ❌ | ❌ |  |
| Formation energies | Bulk Crystals | ❌ | ❌ |  |
| Dimer interactions (S66) | Molecular | ❌ | ❌ |  |
| O₂ / H₂ reaction profiles | Molecules | ❌ | ❌ |  |
| Torsion curves | Molecules | ❌ | ❌ |  |
| S24 (molecule–surface) | Surfaces | ✅ | ✅ | PBE-BJD3 |
| OC20 | Surfaces | ✅ | ✅ | PBE-BJD3 |
| QMOF | MOFs | ✅ | ✅ | PBE |
| RDF/density of water | Liquids | ✅ | ✅ | Experiment / PBE-D3 |


---

## Electrostatic Paper Benchmarks

### Main group thermo-chemistry
| Test Name | Implemented? | Script Ready? | Level of Theory |
|-----------|--------------|---------------|-----------------|
| GMTKN55 | ❌ | ✅ | CCSD(T) |
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
| S30L | ✅ | ✅ | DLPNO-CCSD(T)/CBS |
| LNCI16 | ✅ | ✅ | ωB97X-3c |
| PLA15 for protein fragments interaction energies (full active sites) | ✅ | ✅ | MP2-F12 + DLPNO-CCSD(T) |
| PLF547 for protein fragments interactions | ✅ | ✅ | MP2-F12 + DLPNO-CCSD(T) |
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
| Minnesota database | ❌ | ✅ |  |
| CARBO33 carbocation relative energies and some reactions involving bigger systems | ❌ | ✅ |  |






