# iisgm-bioinfo-test

Aptitude test for IiSGM Microbial Genomics candidates

## Instructions

You are required to calculate SNP distance between those 26 _M. tuberculosis_ isolates provided :microbe:.

The input files are in VCF 4.2 format, obtained with [GATK](https://gatk.broadinstitute.org/), but all information about the parameters are included within the file.

- [Python](https://www.python.org/) language **is required** to complete this test
- [Pandas library](https://pandas.pydata.org/) is strongly adviced

## Submission

- You can send the assignment directly to sergio.buenestado@gmail.com in whichever comprised format suits you

### Iteration 0 | Download repository

You can download this repository with the data included using the terminal (CLI) or as .zip

### Iteration 1 | Parse VCF files to table/dataframe

In data folder you can find all VCF

Create a function to read a single VCF

### Iteration 2 | Extract relevant information from parsed VCF

_M. tuberculosis_ in a haployd organism but those were called (variant calling step) as diploid, hence you will see the usual diploid genotyping (0/0, 0/1, 1/1).

With the correct information analysed, filter the SNPs actually present on each sample, this can be a different function.

### Iteration 3 | Combine present SNP into a presence matrix

Merge extracted information into a matrix to keep track of relevant info such as:

- sample name
- Position
- Mutation (Reference allele and Alternate allele)

The preferred format is a binary Presence/Absence matrix

### Iteration 4 | Calculate the SNP distance between all samples

Determine the pairwise distance between each pair of samples

### Iteration 5 | BONUS - Include INDELS

We have been using the term SNP distance but INDELS are also useful as phylogenetic marker

Add subtle changes to the functions to include INDELS in the distance calculation

### Iteration 6 | BONUS - Represent distance in a phylogenetic tree

You can represent this distance in a dendrogram, using any method you find suitable.

To follow along with the matrix format and the use of python, you are encouraged to use [Scipy library](https://www.scipy.org/), specifically [linkage](https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html#scipy.cluster.hierarchy.linkage) and [dendrogram](https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.dendrogram.html#scipy.cluster.hierarchy.dendrogram)

# :muscle:
