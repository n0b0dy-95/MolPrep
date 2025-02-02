# MolPrep Utility Application
	"A Python utility tool for preparing and refining molecular geometries using RDKit."

#Version:
	0.3.0

# Introduction to MolPrep
	MolPrep is a powerful utility application designed to streamline the preparation and refinement of molecular geometries. With the help of RDKit, this tool enables users to load, clean, standardize, and optimize molecular structures effortlessly. Its robust design ensures scalability and efficiency, making it ideal for chemoinformatics workflows.

# Features at a Glance
	- Flexible File Loading: Supports loading molecular data from .sdf files.
	- Automated Salt Removal: Easily desalt molecular structures to simplify chemistry workflows.
	- Molecule Standardization: Standardize structures using RDKit's MolStandardize module.
	- Geometry Optimization: Optimize molecular geometries using force fields like UFF and MMFF.
	- Parallel Processing: Leverage multiple CPU cores for high-throughput molecule optimization.
	- Customizable Parameters: Fine-tune optimization steps, force field types, and thresholds.

# Prerequisites
	Before using MolPrep, ensure you have the following installed:

# Installation and Setup
	MolPrep is available as a precompiled executable for both Linux and Windows. No manual dependency installation is required.

	- Windows

		1. Download MolPrep.exe from the release page.

		2. Place the executable in a desired directory.

		3. Open a command prompt (cmd) and navigate to the directory.

		4. Run MolPrep.exe --help to view available options.
	
	-Linux

		1. Download MolPrep (Linux executable) from the release page.

		2. Grant execution permissions: $ chmod +x MolPrep

		3. Run: ./MolPrep --help to view available options.

# Example Usage
	- Windows: MolPrep.exe --input Sample_input_diverse.sdf --output optimized_molecules.sdf --optimize --ncpu 4 --forcefield mmff94 --maxstep 300 --nonbondedthreshold 50.0
	
	- Linux: ./MolPrep --input Sample_input_diverse.sdf --output optimized_molecules.sdf --optimize --ncpu 4 --forcefield mmff94 --maxstep 300 --nonbondedthreshold 50.0
	
# N.B.: Can be used in cmd with/without administrator mode.
	
# Command-line options
	--input <file>: Input .sdf file containing molecular structures.

	--output <file>: Output .sdf file for processed molecules.

	--optimize: Enables geometry optimization.

	--ncpu <int>: Number of CPU cores to use (default: all available cores).

	--forcefield <type>: Force field type: uff, mmff94, or mmff94s (default: mmff94).

	--maxstep <int>: Maximum optimization steps (default: 500).

	--nonbondedthreshold <float>: Non-bonded threshold for MMFF optimization (default: 100.0).

# for detailed usage use: 
	-Windows:
		$ molprep.exe -h/--help
	
	-linux:
		$ ./molprep -h/--help

# About the Author
This project was created by SUVANKAR BANERJEE. You can explore the project further and contribute via GitHub: MolPrep on GitHub.

# License
MolPrep is released under the MIT License, fostering open and collaborative software development.

# Acknowledgments
A heartfelt thanks to the RDKit community and all contributors for their invaluable resources and support. Your inspiration drives innovation!
