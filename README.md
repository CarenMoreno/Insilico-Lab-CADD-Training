# Insilico-Lab-CADD-Training
Repository documenting work The Insilico Lab 3-Week (-).

# Insilico Lab - CADD Training (Cohort 5)
Repository documenting my work in The Insilico Lab's 3-Week Virtual Training in Computer-Aided Drug Design (CADD), Cohort 5 (July 2026). Covers protein/ligand preparation, molecular docking, ADMET screening, and AI-based structure prediction, using PyMOL, UCSF Chimera, RCSB PDB, and proteins.plus.

## 📅 Training Overview
- **Program:** The Insilico Lab, 3-Week Virtual Training in CADD
- **Cohort:** 5
- **Dates:** July 3 – July 19, 2026
- **Tools used:** PyMOL, UCSF Chimera, RCSB PDB, proteins.plus (DoGSiteScorer), AlphaFold3

## 📂 Repository Structure
```
Insilico-Lab-CADD-Training/
|
├── Week1_Protein_Target_Selection/
│   ├── Task1_Structure_Selection/
│   ├── Task2_Binding_Site_Analysis/
│   ├── Task3_Protein_Preparation/
│   └── screenshots/
├── Week2_.../
├── Week3_.../
└── README.md   
```

## 🧬 Week 1 - Protein Target Selection, Binding Site Analysis & Preparation

**Target:** Human Dihydrofolate Reductase (DHFR) - PDB ID [1U72](https://www.rcsb.org/structure/1U72)
<p align="center">
  <img src="Week1_Protein_Target_Selection/screenshots/rcsb.structure1U72.png" width="300">
</p>

### Task 1 - Structure Selection
- Resolution: 1.90 Å (X-ray diffraction)
- Ligand: Methotrexate (MTX), cofactor NADPH
- [Screenshot 1 - full protein view]
- [Screenshot 2 - ligand in binding pocket]

### Task 2 - Binding Site Analysis
- Tool: DoGSiteScorer
- Top pocket: P_0 (Drug Score 0.81)
- Key residues: Ile7, Glu30, Phe31, Phe34, Val115, Tyr121, Arg70
- [Screenshot 3 - labeled binding pocket]

### Task 3 - Protein Preparation
- Cleaned in UCSF Chimera (waters removed, hydrogens/charges added via Dock Prep)
- Output: `1U72prepared.pdb`
- [Screenshot 4 - before] / [Screenshot 5 - after]

## 🧬 Week 2 - Drug-likeness Screening, Molecular Docking & ADMET Prediction

**Compounds:** Curcumin ([CID 969516](https://pubchem.ncbi.nlm.nih.gov/compound/969516)), Gefitinib ([CID 123631](https://pubchem.ncbi.nlm.nih.gov/compound/123631)), Kaempferol ([CID 5280863](https://pubchem.ncbi.nlm.nih.gov/compound/5280863))
**Target:** Human DHFR - PDB [1U72](https://www.rcsb.org/structure/1U72) (prepared structure from Week 1)

### Task 1 - Drug-likeness Screening
- Tool: SwissADME (Lipinski's Rule of Five)
- Result: all three compounds passed with 0 violations
- [Screenshot - SwissADME Lipinski results]

### Task 2 — Molecular Docking & Interactions
- Tools: PyRx (AutoDock Vina), BIOVIA Discovery Studio
- Best docking scores (kcal/mol):
  - Gefitinib: **-9.4**
  - Curcumin: -9.0
  - Kaempferol: -8.7
- Gefitinib showed a distinct halogen bond (fluorine) contributing to its top score
- [Screenshot — PyRx docking results]
- [Screenshots — 2D interaction diagrams (Curcumin / Gefitinib / Kaempferol)]

### Task 3 — ADMET Prediction
- Tool: ADMET-AI
- Gefitinib showed the most favorable overall profile: high oral bioavailability, complete intestinal absorption, and strong BBB penetration
- [Screenshot - ADMET-AI summary]

## 🔗 LinkedIn Posts
- Week 1: [link]
- Week 2: [link to your post]

## 🔗 LinkedIn Post
[[Post LinkedIn]](https://www.linkedin.com/posts/carenmoreno-biotech_cadd-drugdiscovery-computationalbiology-activity-7480986480912543744-KnuO?utm_source=share&utm_medium=member_desktop&rcm=ACoAAEsbrkQBSPdKimnT3ne9nmTt0Sueta1viM4)
