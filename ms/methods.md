RLO exposure and sampling

Black abalone, Haliotis cracherodii, (mean shell length = 51.24 mm) from Carmel, California, USA (n = 18) were collected in 2006 and transported to the University of Washington’s Pathogen Containment Facility in Seattle, WA, USA. Abalone were treated with oxytetracycline (OTC) via a 12% TM-100 medicated feed (Phibro Animal Health Corp., Teaneck, NJ, USA) to eliminate any pre-existing RLO infections and allowed to deplete the antibiotic until digestive gland OTC levels were < 10 ppm, a level shown to allow re-infection by the RLO (Friedman et al. 2003). For the duration of the experiment abalone were held in recirculating seawater systems at 19°C, a temperature known to augment RLO transmission and induce WS development (Tissot 1995, Friedman et al. 1997, 2002), and allowed daily access to macroalgae. 
Abalone (n = 9) were exposed to the RLO for 60 days via effluent from a head tank housing RLO infected red abalone, providing an equivalent dose of the non-culturable pathogen to each tank. Control animals (n = 9), held under identical conditions, were exposed to effluent from uninfected red abalone. After 60 days of exposure, red abalone head tanks were removed and black abalone held under constant conditions for 14 months. Upon termination, digestive gland tissues were aseptically excised and stored at -80°C for transcriptomic analyses. All abalone used in the experiment were confirmed infected or uninfected by histology and PCR (Andree et al. 2000).

RNA isolation and library construction 

Total RNA was isolated from digestive gland tissue samples (~20 mg) from RLO exposed (n = 9) and control abalone (n = 9), using a RNA PowerSoil Total RNA Isolation Kit (MoBio Laboratories Inc., Carlsbad, CA, USA). Total RNA was treated with TURBO DNAfree (Life Technologies, Grand Island, NY, USA) according to the manufacturer’s “rigorous” protocol to remove possible genomic DNA carry over. Treated RNA samples were quantified and the removal of genomic DNA was PCR verified. Equal quantities (5 ug) of total RNA from each sample were pooled from the exposed and control treatments. mRNA was isolated from the two pooled samples (RLO exposed and control) with the MicroPolyA Purist Kit (Life Technologies) according to the manufacturer’s protocol. RNA-Seq libraries were constructed using the Whole Transcriptome Analysis Kit (Life Technologies). Briefly, samples were fragmented with RNase III and ribosomal RNA was removed using the Ribominus Concentration Module (Life Technologies). Fragmented mRNA was run on an Agilent Bioanalyzer 2100 using RNA Pico chips/reagents according to the manufacturer’s protocol to verify successful fragmentation (Agilent Technologies, Inc., Santa Clara, CA, USA). The fragmented RNA was then prepared using Adaptor Mix A (for sequencing from the 5’ end) and reverse transcribed. The resulting cDNA was size selected (100-200 bp range) on a Novex 6% TBE-Urea Gel (Life Technologies). In-gel PCR was performed and the amplified DNA was purified using the PureLink PCR Micro Kit (Life Technologies). Yield and size distribution of the amplified DNA was evaluated with DNA 1000 chips on the Bioanalyzer 2100 (Agilent Technologies, Inc.). Templated beads for all libraries were prepared with a 1.5 pM concentration of each library, following the “Full-Scale” protocol in the SOLiD3 Plus System Templated Bead Preparation Guide October 2009 (Life Technologies). Templated bead quality was verified with a workflow analysis run on the SOLiD3 and then sequenced on the SOLiD3 System (Life Technologies).

Sequence read mapping and assembly

raw read QC??? What am I using for this???

XXX was used to remove adapters and low-quality reads from the raw data. The trimmed reads were assembled using Trinity software as described for de novo transcriptome assembly without a reference genome. The two libraries were sequenced, and XX-bp single-end reads were generated. The reads were mapped back onto the assembled transcriptome and read counts for each gene were obtained.

RNA-Seq analysis

For RNA-Seq analysis, expression values were measured as RPKM
(reads per kilobase of exon model per million mapped reads)
(Mortazavi et al. 2008) with an unspecific match limit of 10 and maximum
number of 2 mismatches. Statistical comparison of RPKM
values between the BBC and DH libraries was carried out using Gene expression levels were measured using the reads per kilobase per million reads (RPKM) method using the formula that was previously described by Mortazavi [REF]. A differential expression analysis of the two treatments was performed using the DESeq2 R package (VERSION). Three independent biological replicates for each treatment were analyzed. The p values were adjusted using the Benjamini & Hochberg method. The corrected p value of 0.05 was set as the threshold for significantly differential expression.

RNA-seq analysis was performed to compare differences in gene expression between the digestive gland transcriptome of RLO exposed and control abalone with CLC Genomics Workbench version 6.0 (CLC Bio) using the following parameters: minimum length fraction = 0.9, minimum similarity fraction = 0.8, and maximum number of hits per read = 10. Statistical comparison of  total read counts between the exposed and control libraries was carried out using the R package DESeq (Anders & Huber 2010). Genes were considered differentially expressed when FDR p-values were less than 0.05.
All differentially expressed genes were subjected to GO term enrichment analysis using the Database for Annotation, Visualization and Integrated Discovery (DAVID) v6.7 (http://david.abcc.ncifcrf.gov/; Huang et al. 2009a, 2009b), based on statistical analysis using the Benjamini test. GO terms with p-values less than or equal to 0.05 were considered significantly enriched. Data were visualized on semantic similarity-based scatter-plots using the software REViGO (Supek et al. 2011).

Functional annotation

Consensus sequences from the de novo assembly were compared
to the UniProtKB/Swiss-Prot database (http://uniprot.org) using
the BLAST algorithm (Altschul et al., 1990). A cutoff E-value of 1E-
05 was used for annotations. Associated GO terms (Gene Ontology
database: http://www.geneontology.org) were used to categorize
genes into parent categories and were assigned a functional group
based on the MGI GO Slim database (URL: http://www.informatics.
jax.org). The MGI GO Slim terms for ‘other biological processes’ and
‘other metabolic processes’ are not included in this analysis.




SQLShare was used for analysis (i.e. table joins) during annotation and
RNA-Seq analysis (REF). RNA-Seq analysis was performed using the consensus sequences from de novo assembly of SOLiD reads.

In order to identify enriched biological themes and GO terms, the
Database for Annotation, Visualization and Integrated Discovery
(DAVID) v6.7 was used (Huang et al., 2009a,b). Specifically, corresponding
UniProt accession numbers for differentially expressed
genes were used as the gene list, and compared to a complete list of
the corresponding UniProt accession numbers of the respective transcriptome
(i.e. results of de novo assembly or reference mapping) for
the background. Biological Process terms (DAVID ‘BP Level 2’ categories)
were considered significantly enriched when the p-value was
less than 0.05.

Validation of DEGs by quantitative PCR

Transcripts of interest were selected for qPCR analysis of individual abalone samples from each treatment (exposed = 9; control = 9) to corroborate RNA-Seq results. Transcripts were selected based on their putative role in XXX. For these samples, 1 ug of total RNA from each individual was reverse transcribed using M-MLV Reverse Transcriptase (Promega Corp., Madison, WI, USA) and oligo dT primers (Promega Corp.), following the manufacturer's protocol. Quantitative PCR was performed using 1 uL of cDNA in a 25 uL reaction containing 1x of Sensimix Master Mix (1.5 mM MgCl2; Bioline USA Inc., Taunton, MA, USA), 0.2 uM forward primer, 0.2 uM reverse primer and 2 uM SYBR® Green I (Bioline USA Inc.). Thermal cycling and fluorescence detection were performed using a CFX96™ Real-Time PCR Detection System (Bio-Rad). Cycling parameters were as follows: 95°C for 7 min; 40 cycles of: 95°C for 10 s, 60°C for 30 s, 75°C for 30 s, with fluorescence reads at the end of each cycle. A melt curve analysis was used to verify single amplicons and all samples were run in duplicate. NEED TABLE W/ PRIMERS, SEQ, & GENBANK #

Quantitative PCR analysis was performed using Real-time PCR Miner (Zhao & Fernald 2005). Quantification was performed by calculating the relative mRNA concentration (R0) for each gene for each individual. Briefly, this was calculated using the following equation: R0 = 1/(1+E)^Ct, where E is the average gene efficiency and Ct is the cycle threshold number. The R0 for each gene was normalized to a control (NEC1_RAT) (contig xxx used bc it was not diff expressed across libraries )R0 from each individual. Using the normalized R0, fold increase over the minimum R0 value for each gene was calculated for all individuals. Two-tailed Student’s t-tests were carried out to determine significant differences in expression (p≤0.05; SPSS).
