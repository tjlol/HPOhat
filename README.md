# HPOhat
HPOhat is a genome-wide gene prioritization method, that takes seed genes (known disease-related genes) as inputs, searches and prioritizes candidate disease-associated genes. It integrates more than 15 types of genomic data, including protein-protein interactions (PPIs), co-expression data, biological pathways, phenotype ontology, etc. Based on the data fusion strategy, HPOhat applies random forest algorithm for gene prioritization. HPOhat reaches a high performance and a fast speed for gene prioritiztion comparing with other methods.

### Environment
Linux system

### Download database
Due to the limit of the file size on Github, we compress and split the database. You can download these two split files and merge them into one database file named "gene.data".

`cat HPOhat.tar.bz2.aa HPOhat.tar.bz2.ab| tar xj`

### General Use Case
This software can be used in one of three scenarios:

1. Ideally, you have a list of known disease-related genes (called seed genes) and a list of potential candidate disease variants that overlap gene space and you want to narrow down the list of variants by prioritizing candidate disease genes. 
2. You do not have variants, but you have seed genes and would like to get some candidate genes for your disease that you may want to target sequence, as it is much cheaper than whole-genome or whole-exome sequencing.
3. You have an interest in exploring candidate genes in other fields, such as drug resistance, pathway involving, etc..

### Input files
Input files to HPOhat should contain gene name list, showing in example folder.

### Run the code
One can run the code using the following command after configuring the environment and downloading the data.

`./hpohat input output database/gene.data`

