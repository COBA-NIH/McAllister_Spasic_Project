# Project outline

## <ins>Description of the image sets</ins>
## Dataset 1: CD8-SMA-tumors
The dataset comprises High-contrast images [single-channel grayscale images; DAPI (DNA), FITC (CD8+ T-cells), Texas Red (SMA+ fibroblasts)], Low-contrast images [single-channel grayscale images; DAPI (DNA), CD8 (immune cells), SMA (fibroblasts)], and Other images [single-channel grayscale images; DAPI (DNA), CD8 (immune cells), SMA (fibroblasts), along with a merged image].

### The goals are to quantify:
1) The number of CD8+ cells
2) The % area of tissue that is SMA+
3) Distance association of CD8+ cells and SMA+ cells, i.e., measutrement of the average dustance of CD8+ cells from nearest SMA+ cell, and the number of CD8+ cells within a given distance (20, 50, 100, and 200 um) of SMA+ cells

### Challenges
1) Variations in the staining intensity of SMA
2) Accurate segmentation of fibrillar, non-circular objects

## Dataset 2: CD3-FOXP3-tumors
The dataset comprises merged images (?multiple ROIs from same tumor), and single-channel grayscale images - DAPI (DNA), Cy5 (CD3+ T-cells), FITC (FOXP3+ T-cells).

### The goals are to quantify:
1) The number of CD3+ cells
2) The number of CD3/FOXP3 double-positive cells and % of CD3+ cells that are CD3/FOXP3 double-positive (FOXP3 single-positive cells should not be counted)

### Additional points
 - Ability to use the pipeline regardless of fluorophore for each stain

