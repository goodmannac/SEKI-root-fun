# SEKI-root-fun
Data managment for identification and analysis of root-associated fungal communities, recovered from Pinus lambertiana roots in Sequoia and Kings Canyon National Parks, sampled in 2024. 

## "Extractions" folder
- "Qubit Results - raw_sample_results.csv" is DNA extract quantification data downloaded from the Bogar Lab google drive.
### "dilutions" folder 
- "dna_dilutions_all.Rmd" Takes DNA concentration data from qubits of root extraction products and their dilutions (where original concentration was too high to be read by qubit), calculates concentration of original extraction product, calculates pipetting volumes to dilute extraction products to 2ng/ul in preparation for our library prep protocol. 
- "Results/DNA_dilutions_all_striptubes.csv" is most complete/useful output file. 
### "extraction_metadata" folder 
- "make_extraction_metadata_w_dilutions.Rmd" makes most useful/complete extraction metadata csv, "Results/extraction_metadata_w_dilutions.csv". This script takes DNA_dilutions_all_striptubes.csv from dilutions folder and joins with root sampling and grinding metadata. Tidies notes from AG's Feb 2026 inventory of extra root grounds and joins this to metadata as well.
- "EM Metadata entry, SEKI 2024 - PILA.csv" is root sampling and grinding metadata downloaded from the Bogar Lab google drive.
- "EM Metadata entry, SEKI 2024 - AG_direct_edit_22April2026.csv" is root sampling and grinding metadata downloaded from the Bogar Lab google drive, with Anna's April 2026 modifications correcting sample labeling mistakes. Extensive justification for these edits in Anna's OneNote.
- "EM Metadata entry, SEKI 2024 - Xtra grounds volume.csv" contains notes from Anna's Feb 2026 inventory of extra root grounds. 
- "qubit_results_exploration.Rmd" investigates extraction yields; highlights too-high or too-low reads that need attending to and quickly compares DNA yields to experimental factors