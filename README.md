# Masterclass-Hackathon

## Introduction
A simple baseline provide training and validation script to predict mutation from the H&E stained whole slide images. This pipeline reproduces the results reported in [1, 2].

![](/fig/fig.png)
 
## Dataset requirements
1.	Tumor region of H&E stained whole slide images tiled into blocks of size 512 by 512, arranged in a separate directory per whole slide image.
2.	A lib_train.csv where each row contains: 
a.	“SLIDES”: are the names of directories where whole slides image are stored as tiles of size 512 by 512
b.	“Mutation”: is the label information for each slide (1 for mutation present, 0 otherwise)
Sample train and test set csv  files are provided in the “data” folder of this repository.
This implementation is also inspired from and reuses few routines from another github repository [3] which contains implementation of Campanella et al. 2019. 

## References:
1.	Kather, J.N., Pearson, A.T., Halama, N. et al. Deep learning can predict microsatellite instability directly from histology in gastrointestinal cancer. Nat Med 25, 1054–1056 (2019) doi:10.1038/s41591-019-0462-y
2.	Kather, J.N., Lara, R. Heij, et al. Pan-cancer image-based detection of clinically actionable genetic alterations. bioRxiv 833756; doi: https://doi.org/10.1101/833756
3.	MIL-nature-medicine-2019.https://github.com/MSKCC-Computational-Pathology/MIL-nature-medicine-2019

