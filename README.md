# Rhizobia_EPS_Manuscript
This repository has the data from the paper named: "Natural Sinorhizobium meliloti isolates with dry colonies tend to have higher soil fitness but lower host fitness and benefit than mucoid isolates"

Phenotype/

Has the information of the soil and plant host experiments. The code can be found in Analysis/; the raw data can be found in Data_input/, and the Tables and Figures generated in this study can be found in Figures/ and Tables/

Genotype/

Has the information on the genome wide association analysis, the phylogenetic tree, and the comparison between pairs. The raw data and the GWAS results are in Data_input/, the code is in Analysis/ and the tables generated in this study and the ones that were used to run the GWAS are in Tables/. The GWAS was run in the shell, but the documents used are available in this repository. 

Several files used in this study were generated in the manuscript Guha et al., (2026) currently under review, but all the ones that were used in this study are available in this Github repository. 


### How to reproduce the analysis ###

We are using renv to record the exact packages used in this analysis 
We are using Version 2026.09.0+174 (2026.09.0+174)

1. Clone this repository
2. Open the "Rhizobia_EPS_Manuscript.Rproj" in the repository root of R studio
3. Then in the console run "renv::restore()" and then type y.
4. Knit the analysis.
5. There is one big file that is not present: strain_118_variants.vcf. However in Genotype/Data_input/ we have the compressed version "strain_118_variants.vcf.zip" that is used in the code Phenotype/Analysis/ in the Rmarkdown MucoidEPS_ManuscriptRmd.Rmd because it is pivotal when accounting for population structure

