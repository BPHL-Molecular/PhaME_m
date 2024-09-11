# PhaME_m
The debugging version of PhaME (Phylogenetic and Molecular Evolution analysis tool). PhaME_m retains all the functions of PhaME, namely performing phylogenetic and molecular evolutionary analysis from sequencing reads, draft assemblies or completed genomes. The sequencing data in FASTQ or FASTA format can be directly inputted. 

# Why PhaME_m?
Since PhaME has not been updated for a long time, the existing versions (precompiled, development, and docker versions) have some issues on installation or running. PhaME_m debugs these issues. Following the installation guide below, the PhaME can be successfully installed and run on a local machine. 

# How to install?
1. Create a separate conda environment and then activate it:
   ```bash
   conda create -n phame_m
   ```
   ```bash
   conda activate phame_m
   ```
2. Install required dependencies in the "phame_m" conda environment:
   ```bash
   mamba install perl-bioperl
   mamba install samtools
   mamba install bcftools
   mamba install mummer
   mamba install bowtie2
   mamba install fasttree
   mamba install bbmap
   mamba install raxml
   mamba install perl-parallel-forkmanager
   mamba install perl-statistics-distributions
   mamba install paml
   mamba install mafft
   mamba install hyphy
   ```
3. Clone the github repo of PhaME:
   ```bash
   git clone https://github.com/LANL-Bioinformatics/PhaME.git
   ```
5. Test if the installation was successful:
   ```bash
   cd PhaME
   bash ./test/TestAll.sh 1
   ```
# FAQ
1. ERROR: It makes no sense to perform bootstrap with less than 4 sequences.
2. ERROR: Alignment must have at least 3 sequences.

# More about PhaME:
1. The github repo:    
   https://github.com/mshakya/PhaME/tree/master
2. Docs: https://phame.readthedocs.io/en/latest/index.html
3. The publication:   
   Shakya, M., Ahmed. S.A, Davenport K.W., Flynn M.C., Lo. C-C, Chain P.S.G. Standardized phylogenetic and molecular evolutionary analysis applied to species across the 
   microbial tree of life. Sci. Rep. 10, 1723 (2020).
