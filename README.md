# Transposon-insertion-site-identification
Transposon mutagenesis is widely used for determining gene functions in molecular biology. Traditionally, after mutagenesis, laborious 2-step PCR processes (like nested PCR) are used for identifying which gene has been inserted in the mutated phenotype. 
This script takes in fastq sequencing file and transposon sequences and returns a list of reads that have been inserted by transposons, with transposon cut off. Users can then map these reads to the target genome and view it. Blast is also worth trying. Local alignment algoritm is used to search for insertion pattern. It is done without mapping raw reads to the genome. 
All the functions are written in base R, so no additional packages are needed. 
It is recommended to use Rsubread to do the mapping.
