#Speculative SNP Prediction

One idea we can try to persue is predicting whether a new SNP not associated
with AMR might be involved in AMR based on where it occurs in the gene.

The loose idea for this is to mimic a kernel density estimate 

- Take all recorded SNPs and center fairly wide discrete gaussians over them

- Combine distributions across whole gene for a 'mutation importance' distribution
for the gene

- Report any gene that falls into this area.

Analysis
--------

- Get CARD data `get_data.sh` (version 2.0.3) for this analysis as it stands

- Focus on just ribosomal for now 
