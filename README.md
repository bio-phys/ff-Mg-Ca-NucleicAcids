# ff-Mg-Ca-NucleicAcids
(https://aip.scitation.org/doi/full/10.1063/5.0048113) Extension for the interactions with DNA and RNA of our previously bulk-optimized force field parameters (https://doi.org/10.1063/1.5017694) 

## Introduction
******************
Previously, we have developed force field parameters for the metal cations in combination with the TIP3P water model.
Here, we extend the applicability of the parameters for Mg2+ and Ca2+  to correctly describe their interactions with DNA and RNA in biomolecular simulations by including experimental binding affinities toward the phosphate oxygen. 

The improved parameters improved the agreement of the binding affinities and resulted in an improvement of structural properties of the bound ions in the experimental structures.

The advantage of the current approach is that it leaves the ion-water and ion-ion interactions unchanged and can therefore be transferred easily to other ion binding sites on biomolecules.

## Quick start guide
******************
Our parameters are optimized for the TIP3P water model.
The parameters work in combination with RNA (Amber99sb-ildn* + parmbsc0 +a χ0L3)  and DNA (Amber99sb-ildn* + parmbsc1) force fields .
For Mg2+ and Ca2+ interacting with the atom type  O2, the Lorentz-Berthelot combination rule is modified.
Note that we have chosen unique names for the optimized parameters to avoid errors in overwriting atom names:
* CXY - Cl
* Mg2 - MG
* Ca2 - CA


## Example: Double stranded DNA (PDB-id: 477D) in 0.06 M of CaCl2
******************
The folder example_477d contains all files for an MD simulation with GROMACS of a 12-bp double-stranded DNA (PDB-id: 477D) with the optimized parameters.
Initial coordinates are given in 477d.gro.

## Citation
******************
If you use our optimized parameters for Mg2+ and Ca2+ optimized for the interactions with nucleic acids, please cite:

S. Cruz-León, K. K. Grotz  and N. Schwierz, J. Chem. Phys. **154**, 171102 (2021)
https://aip.scitation.org/doi/full/10.1063/5.0048113


Implementation has been tested by Sergio Cruz-León and Kara K. Grotz.
USE AT YOUR OWN RISK!!
