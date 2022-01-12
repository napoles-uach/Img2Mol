## Overview
 Here we provide the benchmark datasets that was used to evaluate the performance of Img2Mol and compare it with that of state-of-the-art molecular recognition methods. The following benchmark datasets (all 8-bit grayscale images) were used.
 
### Img2Mol
Test set collection of 25[thin space (1/6-em)]000 images and molecule descriptions. Images were generated as described in subsection 3.3. The resolution of the images is 224 × 224 px. Only half of our original test set is used due to the computational time of the baseline methods. The data set consists of typical small molecules with an average size of 25 atoms, ranging between 6 and 44 atoms.
### STAKER
The validation set collection of 30[thin space (1/6-em)]000 images and molecule descriptions provided by Staker et al.12 The images are based on US Patent Office (USPTO) data. The image resolution is 256 × 256 px. Molecules are composed of 24 atoms on average, ranging from 7 at the minimum to 51 at the maximum.
### USPTO
A collection of 4852 images and molecule descriptions based on US Patent Office (USPTO) data, obtained from Rajan et al.11 The average resolution of the images is 649 × 417 px. The dataset consists of molecules with an average size of 28 atoms, ranging between 10 and 96 atoms.
### UoB
5716 images and molecule descriptions of chemical structures developed by the University of Birmingham, obtained from Rajan et al.11 The average resolution of the images is 762 × 412 px. The molecules in this data set are quite small, consisting on average of only 13 atoms, ranging between 4 and 34 atoms.
### CLEF 
A collection of 711 images and molecule descriptions based on the Conference and Labs of the Evaluation Forum (CLEF) test set, obtained from Rajan et al.11 The average resolution of the images is 1243 × 392 px. The dataset consists of molecules with an average size of 26 atoms, ranging between 4 and 42 atoms.
### JPO
A collection of 365 images and molecule descriptions based on Japanese Patent Office (JPO) data, obtained from Rajan et al.11 Note that this data set contains many textual labels, including Japanese characters, and irregular features, including line thickness variations. In addition, some images are characterised by poor quality. The average resolution of the images is 607 × 373 px. Molecules are composed of 20 atoms on average, ranging from 5 at the minimum to 43 at the maximum.


For the smaller benchmark datasets (USPTO, UoB, CLEF and JPO), we applied a slight input perturbation by adding rotation (randomly drawn from [−5°, 5°]) and shearing (xy-shearing factor randomly drawn from [−0.1, 0.1]). Every input image of those benchmarks is perturbed five times randomly. This is done in order to detect potential overfitting of the baseline methods to those small, well known datasets.