# get_longest_CDS_per_gene

The script get_longest_CDS_per_gene.py is written in Python3 and require the module Biopython. The program extracts the longest coding sequence (CDS) per gene.

To run this script use the following command structure:
python get_longest_CDS_per_gene.py --input_fasta input_CDS.fas --input_table table_geneID_transcriptID --output_file output.fas

input_fasta: Fasta file with a set of CDSs. That file should be obtained by using gffread (Pertea and Pertea 2020). The header should look like:
```
>rna-XM_054099293.1
```

input_table: A tab delimited file containing the following information:locusID (gene identificator) and transcriptID. This file must be sorted by the first column. It should look like:
```
LOC128854707  XM_054089416.1
LOC128854708  XM_054089018.1
LOC128854710  XM_054089015.1
LOC128854711  XM_054089016.1
LOC128854712  XM_054089017.1
LOC128854712  XM_054089019.1
LOC128854712  XM_054089020.1
```

output_file: Set of the resulted longest CDS per gene in fasta format.
