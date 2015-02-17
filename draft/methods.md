Sequence read mapping and assembly

Library sequencing was performed on the SOLiD3 System (Life Technologies) and CLC Genomics Workbench version 6.0 (CLC Bio) was used to remove adapters and low-quality reads from the raw data. The trimmed reads were assembled using Trinity software as described for de novo transcriptome assembly without a reference genome.

Functional annotation

Consensus sequences from the de novo assembly were compared to the UniProtKB/Swiss-Prot database (http://uniprot.org) using the BLAST algorithm (Altschul et al. 1990). A cutoff e-value of 1E-05 was used for annotations. SQLShare was used to join annotation results with associated GO terms (http://www.geneontology.org) to categorize genes into parent categories and assign them a functional group based on the MGI GO Slim database (http://www.informatics.jax.org). The MGI GO Slim terms for ‘other biological processes’ and ‘other metabolic processes’ are not included in this analysis.

RNA-Seq analysis

RNA-seq analysis was performed to compare differences in gene expression between the digestive gland transcriptome of RLO exposed and control abalone with CLC Genomics Workbench version 6.0 (CLC Bio) using the following parameters: minimum length fraction = 0.9, minimum similarity fraction = 0.8, and maximum number of hits per read = 10. Expression values were measured as RPKM (reads per kilobase of exon model per million mapped reads, Mortazavi et al. 2008) with an unspecific match limit of 10 and maximum
number of 2 mismatches. Statistical comparison of total read counts between exposed and control libraries was carried out using the R package DESeq2 (Love et al. 2014). Genes were considered differentially expressed when p-values were less than 0.05. All differentially expressed genes were subjected to GO term enrichment analysis using the Database for Annotation, Visualization and Integrated Discovery (DAVID) v6.7 (http://david.abcc.ncifcrf.gov/, Huang et al. 2009a, 2009b) based on statistical analysis using the Benjamini test. GO terms with p-values less than or equal to 0.05 were considered significantly enriched. Data were visualized on semantic similarity-based scatter-plots using the software REViGO (Supek et al. 2011).







