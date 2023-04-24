# DATA AND CODE RELATED TO SIMULATED SINGLE-CHAIN NANOPARTICLES

This repository contains a set of example scripts and data related to the morphologies of single-chain nanoparticles as formed from reactive precursor chains. Configurations of SCNP morphologies are distributed separately due to space constraints. 

This content is available under CC BY NC 4.0 License.

## REFERENCES

The specific application, data, and models are described in 

Patel, R.A.; Colmenares, S.; Webb, M.A.; ``Sequence Patterning, Morphology, and Dispersity in Single-chain Nanoparticles: Insights from Simulation and Machine Learning'' DOI: 10.26434/chemrxiv-2023-ss7f4-v2

## FILE DESCRIPTION

### data

The `data' directory includes three files. 
-`SCNP_sequences.txt' is a plain-text, human-readable file that enumerates the sequences for all of the precursor chains simulated; there are 320 lines in this file. 
-`SCNP_dataset.csv' contains all the meta-data and derived properties of formed single-chain nanoparticles. There are 320*24 = 7680 data lines in this file and one header file. 

### lammps
The `lammps' directory includes 7 files.
-`in.data' - an example LAMMPS data file for sequence 0 (f = 0.1, \beta = 0.2)
-`in.lammps' - an example LAMMPS input script used to generate 24 independent snapshots of the equilibrated chain
-`react.data' - an example LAMMPS data file of the 0th independent snapshot obtained from running in.lammps
-`react.lammps' - an example LAMMPS input file used to react the precursor into a SCNP
-`sys.data.endreact' - an example LAMMPS data file obtained after the SCNP is finished reacting
-`prod.lammps' - an example LAMMPS input file used to equilibrate and gather statistics on the structure
-`WCA.txt' - an example of the WCA potential implemented as a tabulated potential, used by react.lammps and prod.lammps
