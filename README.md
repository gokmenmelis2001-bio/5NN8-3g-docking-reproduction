# 5NN8–3g Docking Reproduction

This repository documents an independent reproduction of the published molecular docking workflow for compound **3g** against human acid alpha-glucosidase (**rhGAA**, PDB ID: **5NN8**).

The aim is to reproduce the reported binding region, docking score, and key active-site interactions using an independently prepared docking workflow.

## Reference Study

Gezer D., Ozyıldız Z., Gokmen Z., et al.  
**Novel 1H-pyrrole-2,5-dione derivatives as potential anti-diabetic agents: design, synthesis, in vitro, in ovo, and molecular docking studies.**  
*Bioorganic & Medicinal Chemistry Letters.* 2026;139:130710.  
DOI: 10.1016/j.bmcl.2026.130710

## System

- **Protein:** Human acid alpha-glucosidase (rhGAA)
- **PDB ID:** 5NN8
- **Ligand:** Compound 3g
- **Docking software:** AutoDock Vina
- **Strategy:** Blind docking followed by focused docking

## Published Docking Result

The reference study reported compound **3g** as the top in silico docking hit against rhGAA.

- **Published focused docking score:** −9.35 kcal/mol
- **Binding region:** Deep catalytic pocket of rhGAA
- **Reported key interacting residues:** ASP404 and ASP616

The study also described the binding mode of 3g as being strongly influenced by hydrophobic packing within the catalytic pocket.

## Independent Reproduction

The docking workflow was independently reproduced using PDB structure **5NN8**.

The workflow included:

1. Protein preparation
2. Ligand preparation
3. Blind docking across the protein surface
4. Identification of the catalytic binding region
5. Focused docking within the catalytic pocket
6. Selection and structural analysis of the top-ranked pose

## Reproduced Result

- **Best focused docking score obtained:** approximately −9.06 kcal/mol
- The reproduced pose was located within the same deep catalytic region reported in the reference study.
- The reproduced binding environment included the published active-site residues **ASP404** and **ASP616**.

## Comparison

| Feature | Published Study | Independent Reproduction |
|---|---|---|
| Protein | rhGAA / PDB 5NN8 | rhGAA / PDB 5NN8 |
| Ligand | Compound 3g | Compound 3g |
| Strategy | Blind → Focused docking | Blind → Focused docking |
| Focused docking score | −9.35 kcal/mol | −9.06 kcal/mol |
| Binding region | Deep catalytic pocket | Deep catalytic pocket |
| Shared key residues | ASP404, ASP616 | ASP404, ASP616 |

Small differences in docking scores can arise from differences in protein preparation, ligand preparation, protonation state, grid definition, and software settings.

## Tools

- AutoDock Vina
- AutoDockTools / MGLTools
- PyMOL
- Discovery Studio Visualizer

## Scope

This repository is limited to the independent reproduction of the **published molecular docking analysis**.

All computational outputs and figures included here are independently generated.

No publisher-owned figures or full-text copies of the reference article are included.

## Disclaimer

Docking scores are computational predictions and should not be interpreted as experimental binding affinities or as proof of biological activity.
