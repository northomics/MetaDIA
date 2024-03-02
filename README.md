# MetaDIA


## Instructions

Please search one raw file at a time against MetaPep database using DIA-NN. The MetaPep database can be downloaded here or the MetaPep article (doi: 10.1016/j.csbj.2023.08.025). Because the workflow will generate a spample-specific database, please be sure only put one raw data a time.


[Download](https://github.com/northomics/MetaDIA/releases/download/Pub/workflow.7z) and extract the workflow and resources


1.Run the GUI by click the start.bat file

2.Set up the resources path

3.Set up the path of MetaPep search Folder (the first search result) and Output folder

4.Specify the parameters you desire. (see detail in the article)

5.Select "Output pep rank table" button to output the rank of peptides with FuncTax and Dectec scores (optional)

6.Click "Run program" button to start. 

Reduced_peptide_database.fasta can be found in the output folder. The peptide_protein file record the the correspondence between peptides and proteins, which can be used for taxonomic and functional analysis. 'analysis_taxa_func.py' recored the method of taxonomic and functional analysis in this article. 

*The total time varies according to the number of threads and computer configuration. On the author's computer (Intel(R) Core(TM) i7-8700 CPU @ 3.20GHz   3.19 GHz), using 8 threads takes approximately 15 minutes.


## Resources:

1.Functional abundance file: function.abundance.possibility.csv in the workflow file

2.Functional annotation folder: The data is downloaded from the UHGP database (version 2.0.2, doi:10.1038/s41587-020-0603-3). Put all [species_accession]_eggNOG.tsv into one file. (https://ftp.ebi.ac.uk/pub/databases/metagenomics/mgnify_genomes/human-gut/v2.0.1/)

3.MetaPepDetec: Please downloaded the database from (https://osf.io/zrgaf)
