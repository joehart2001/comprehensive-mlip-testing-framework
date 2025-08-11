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

### **MACE-MP-0 Tests (Appendix A & B)**
| Test Name | Category | Implemented? | Script Available? | Reference Data? | Level of Theory |
|-----------|----------|--------------|-------------------|-----------------|-----------------|
| Single/di-interstitial defects in Si | Bulk Defects | ❌ | ❌ | ⬜ | DFT (PBE) |
| Amorphous Si from melt–quench | Amorphous | ❌ | ❌ | ⬜ | DFT (PBE) |
| Amorphous Carbon | Amorphous | ❌ | ❌ | ⬜ | DFT (PBE) |
| Ceria nanoparticles | Nanoparticles | ❌ | ❌ | ⬜ | DFT (PBE) |
| Inorganic halide perovskite | Perovskites | ❌ | ❌ | ⬜ | DFT (PBE) |
| Hybrid Organic–Inorganic Perovskites | Perovskites | ❌ | ❌ | ⬜ | DFT (PBE) |
| Protein dynamics & stability | Biomolecules | ❌ | ❌ | ⬜ | MD / Experiment |
| Hydrogen combustion | Reactions / MD | ❌ | ❌ | ⬜ | DFT (PBE) |
| Sulfur polymerisation | Polymers | ❌ | ❌ | ⬜ | DFT (PBE) |
| Zeolites | Porous materials | ❌ | ❌ | ⬜ | DFT (PBE) |
| Open-circuit voltage of lithiated graphite | Batteries | ❌ | ❌ | ⬜ | DFT (PBE) |
| Jahn–Teller distortions in LiNiO₂ | Transition Metal Oxides | ❌ | ❌ | ⬜ | DFT (PBE) |
| Point & extended defects in BCC metals | Bulk Defects | ❌ | ❌ | ⬜ | DFT (PBE) |
| Alumina defects & bulk diffusion | Oxides | ❌ | ❌ | ⬜ | DFT (PBE) |
| Random structure search: As | Structure Search | ❌ | ❌ | ⬜ | DFT (PBE) |
| Bulk & nanoconfined water properties | Liquids | ❌ | ❌ | ⬜ | DFT (PBE) |
| Ethanol–water density–composition curves | Liquids | ❌ | ❌ | ⬜ | Experiment |
| Solvent mixtures | Liquids | ❌ | ❌ | ⬜ | Experiment |
| Aqueous interfaces | Interfaces | ❌ | ❌ | ⬜ | DFT (PBE) |
| Molten salts | Liquids | ❌ | ❌ | ⬜ | Experiment / DFT |
| Room-temperature ionic liquids | Liquids | ❌ | ❌ | ⬜ | Experiment / DFT |
| High-pressure hydrogen | High-Pressure | ❌ | ❌ | ⬜ | DFT (PBE) |
| Ammonia & borane decomposition | Reactions | ❌ | ❌ | ⬜ | DFT (PBE) |
| Heterogeneous catalysis | Surfaces / Catalysis | ❌ | ❌ | ⬜ | DFT (PBE) |
| Carborane rearrangement | Reactions | ❌ | ❌ | ⬜ | DFT (PBE) |
| Transition metal dichalcogenides | 2D Materials | ❌ | ❌ | ⬜ | DFT (PBE) |
| Electrode–electrolyte interfaces | Batteries | ❌ | ❌ | ⬜ | DFT (PBE) |
| MOFs | Porous Materials | ❌ | ❌ | ⬜ | DFT (PBE) |
| Combinatorial materials discovery | Materials Discovery | ❌ | ❌ | ⬜ | Various |
| Alanine tripeptide free energy surface | Biomolecules | ❌ | ❌ | ⬜ | DFT / Experiment |
| Molecule–surface interactions | Surfaces | ❌ | ❌ | ⬜ | DFT (PBE) |
| Computational efficiency test | Performance | ❌ | ❌ | ⬜ | N/A |

---

### **Standardised Benchmarks (Appendix B)**
| Test Name | Category | Implemented? | Script Available? | Reference Data? | Level of Theory |
|-----------|----------|--------------|-------------------|-----------------|-----------------|
| Phonons | Bulk Crystals | ✅ | ✅ | ✅ | PBE |
| Bulk & shear moduli | Bulk Crystals | ✅ | ✅ | ✅ | PBE |
| Cohesive energies (X23, ICE-DMC13) | Molecular Crystals | ✅ | ✅ | ✅ | PBE+D3 / DMC |
| Lattice constants | Bulk Crystals | ✅ | ✅ | ✅ | PBE |
| Reaction barrier heights | Molecules | ⬜ | ⬜ | ✅ | PBE |
| Homonuclear diatomics | Molecules | ✅ | ✅ | ✅ | PBE |

---

### **Planned Additional Benchmarks**
| Test Name | Category | Implemented? | Script Available? | Reference Data? | Level of Theory |
|-----------|----------|--------------|-------------------|-----------------|-----------------|
| EOS metals (various sizes) | Bulk Crystals | ❌ | ❌ | ⬜ | PBE |
| Thermal conductivity | Bulk Crystals | ❌ | ❌ | ⬜ | PBE |
| Formation energies | Bulk Crystals | ❌ | ❌ | ⬜ | PBE / Experiment |
| Dimer interactions (S66) | Molecular | ❌ | ❌ | ✅ | CCSD(T) |
| GMTKN55 (5 categories) | Molecules | ❌ | ❌ | ✅ | Various high-level |
| O₂ / H₂ reaction profiles | Molecules | ❌ | ❌ | ⬜ | PBE |
| Torsion curves | Molecules | ❌ | ❌ | ⬜ | CCSD(T) / PBE |
| X24 (molecule–surface) | Surfaces | ❌ | ❌ | ✅ | PBE |
| OC20 | Surfaces | ❌ | ❌ | ✅ | PBE |
| QMOF | MOFs | ❌ | ❌ | ✅ | PBE |
| RDF/density of liquids | Liquids | ❌ | ❌ | ⬜ | Experiment / DFT |
