Custom Parcellations

A repository of customized versions of various publically available parcellations.
All files created by Benjamin A. Ely unless otherwise noted.
Direct all questions/comments/threats to: benjamin dot ely at einsteinmed dot org


Contents:

bilateral_HCP_Multimodal_Parcellation_32k
-Combines corresponding left and right cortical parcels from the HCP Multimodal Parcellation (180 parcels)
     -Glasser MF et al. Nature 2016
-Also combines left and right major subcortical structures included in standard CIFTI space (10 parcels)
     -NB: Uniquely, the standard CIFTI brainstem structure is already bilateral
-Total of 206 bilateral parcels in 32k CIFTI space
-Files:
     -bilatparc206_grayscale.LRS.dlabel.nii - Grayscale version
     -bilatparc206_Rcolor.LRS.dlabel.nii    - Colored version (uses values from right cortex)

Grayordinate_Masks_32k
-Subsets of Grayordinate space useful for masking/using as templates
     -Tip: To see commands used to generate files, enter `wb_command -file-information <filename> -only-metadata`
-Numbers in filenames indicate the number of grayordinates (i.e. voxels and/or vertices)
Files:
     -Atlas_ROIs_31870_index.32k.S.dscalar.nii     - Standard subcortex label indices (CIFTI format, subcortex only)
     -Atlas_ROIs_31870_index.32k.S.nii.gz          - Standard subcortex label indices (NIFTI format)
     -Atlas_ROIs_31870_label.32k.S.dlabel.nii      - Standard subcortex labels (CIFTI format, subcortex only)
     -Atlas_ROIs_31870_label.32k.S.nii.gz          - Standard subcortex labels (NIFTI format)
     -Atlas_ROIs_31870_ones.32k.S.dscalar.nii      - Subcortex mask (CIFTI format, subcortex only)
     -Atlas_ROIs_31870_ones.32k.S.nii.gz           - Subcortex mask (NIFTI format)
     -CORTEX_LEFT_29696_ones.32k.L.dscalar.nii     - Left cortex mask without medial wall (CIFTI format, left cortex only)
     -CORTEX_LEFT_29696_ones.32k.L.func.gii        - Left cortex mask without medial wall (GIFTI format)
     -CORTEX_LEFT_32492_ones.32k.L.dscalar.nii     - Left cortex mask with medial wall (CIFTI format, left cortex only)
     -CORTEX_LEFT_32492_ones.32k.L.func.gii        - Left cortex mask with medial wall (GIFTI format)
     -CORTEX_RIGHT_29716_ones.32k.R.dscalar.nii    - Right cortex mask without medial wall (CIFTI format, right cortex only)
     -CORTEX_RIGHT_29716_ones.32k.R.func.gii       - Right cortex mask without medial wall (GIFTI format)
     -CORTEX_RIGHT_32492_ones.32k.R.dscalar.nii    - Right cortex mask with medial wall (CIFTI format, right cortex only)
     -CORTEX_RIGHT_32492_ones.32k.R.func.gii       - Right cortex mask with medial wall (GIFTI format)
     -Grayordinates_59412_ones.32k.LR.dscalar.nii  - Bilateral cortex mask without medial wall (CIFTI format, left + right cortex only)
     -Grayordinates_64984_ones.32k.LR.dscalar.nii  - Bilateral cortex mask with medial wall (CIFTI format, left + right cortex only)
     -Grayordinates_91282_ones.32k.LRS.dscalar.nii - Whole-brain mask without medial wall (CIFTI format, left + right + subcortex)
     -Grayordinates_96854_ones.32k.LRS.dscalar.nii - Whole-brain mask with medial wall (CIFTI format, left + right + subcortex)


Naming Conventions:

.32k   = in standard 32k CIFTI Grayordinate space
.L/R/S = includes Left Cortex/Right Cortex/Subcortex structures
_ones  = all grayordinate values set to 1
_index = grayordinate values reflect label index values
_label = grayordinate colors reflect structure labels


References:

Glasser MF et al. A Multi-Modal Parcellation of the Human Cerebral Cortex. Nature, 2016.
