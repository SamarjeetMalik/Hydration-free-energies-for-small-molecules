# Implementation of the paper on FreeSolv: Experimental and Calculated Small Molecule Hydration Free Energies

# Abstract:

This work provides a curated database of experimental and calculated hydration free energies for small molecules in water, along with experimental values and input files. Experimental values are taken from prior literature and will continue to be curated, with updated experimental references and data added as it becomes available. Calculated values are based on the GAFF small molecule force field in TIP3P water with AM1-BCC charges, as in the provided parameter files. Values were calculated using the GROMACS simulation package, with full details given in references cited within the database itself. This database builds on previous work from the Mobley lab and others, and extends the prior database. With deposition in eScholarship, the database is now versioned, allowing citation of specific versions of the database, and easier updates.








# Manifest
- `gromacs_analysis`: Contains plots resulting from GROMACS analysis of some of the data in FreeSolv.
- `gromacs_energies`: Contains XVG files associated with the most recent (2017) update of FreeSolv calculated values; these files are large and are only available in the archived version of the database and not on GitHub.
- `gromacs_mdpfiles`: Contains GROMACS run (.mdp) files used for the calculations connected with the most recent (2017) update of the calculated hydration free energies and enthalpies reported here.
- `mol2files_gaff.tar.gz`: contains mol2 files for all compounds with AM1-BCC charges and GAFF atom types
- `mol2files_sybyl.tar.gz`: contains mol2 files for all compounds with AM1-BCC charges and SYBYL atom types
- `primary-data`: Primary data from which the contents of this database can be re-generated; obtained from full database via `scripts/extract-primary-data.py`
- `scripts`: Scripts pertaining to the material deposited here
- `sdffiles.tar.gz`: SDF-format files for all of the molecules deposited here (as in `mol2files_gaff` and `mol2files_sybyl`)
- `amber.tar.gz`: AMBER format parameter, coordinate, and frcmod files corresponding to the systems we ultimately simulated in GROMACS.
- `gromacs_original.tar.gz`: GROMACS format topology and coordinate files for the calculations associated with the computed values in FreeSolv, for calculations in gas phase. These were generated from AMBER files via acpype, prior to our more recent migration to ParmEd.
- `gromacs_solvated.tar.gz`: GROMACS format topology and coordinate files for the calculations associated with the computed values in FreeSolv, for calculations in solution, again generated from AMBER files via acpype.
- `lammps.tar.gz`: LAMMPS format topology and coordinate files for the calculations associated with the computed values in FreeSolv, automatically converted using InterMol from the AMBER files
- `charmm.tar.gz`: CHARMM format topology and coordinate files for the calculations associated with the computed values in FreeSolv, automatically converted using ParmEd (via InterMol) from the AMBER files
- `gromacs.tar.gz`: GROMACS format topology and coordinate files for the calculations associated with the computed values in FreeSolv, automatically converted using ParmEd (via InterMol) from the AMBER files
- `desmond.tar.gz`: DESMOND format topology and coordinate files for the calculations associated with the computed values in FreeSolv, automatically converted using InterMol from the AMBER files
- `simulation_comparison_input/`: directory containing input files used for the validation of the input conversion files by comparing energy files, description of automated conversion process, and the energy comparisons. See `simulation_comparison_input/README.md` for more details.
- `README.md`: This file
- `database.pickle`: Python pickle file of the FreeSolv database
- `database.json`: JSON format version of the FreeSolv database also stored in `database.pickle`
- `database.txt`: Text format version of some of the fields from the database
- `groups.txt`: Functional groups assigned to the different compounds in the database
- `iupac_to_cid.pickle` and `.json`: Python pickle file and JSON file containing a dictionary for converting IUPAC names to FreeSolv compound IDs
- `smiles_to_cid.pickle` and `.json`: Python pickle and JSON file containing a dictionary for converting SMILES strings to FreeSolv compound IDs
- `notebooks/OrionDB.ipynb`: iPython notebook providing an example of concatenating molecules and associating generic data.



