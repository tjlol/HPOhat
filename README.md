# HPOhat
HPOhat is a genome-wide gene prioritization method, that takes seed genes (known disease-related genes) as inputs, searches and prioritizes candidate disease-associated genes. It integrates more than 15 types of genomic data, including protein-protein interactions (PPIs), co-expression data, biological pathways, phenotype ontology, etc. Based on the data fusion strategy, HPOhat applies random forest algorithm for gene prioritization.

### Environment
Linux system

### Release files
cat HPOhat.tar.bz2.aa HPOhat.tar.bz2.ab| tar xj

### Once the compressed file is extracted, you should move to HPOhat folder and run ./hpohat
./hpohat input output database/gene.data
