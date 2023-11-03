# Project outline

## <ins>Description of the image sets</ins>
## Dataset 1: CD8-SMA-tumors
The dataset comprises High-contrast images [single-channel garyscale images; DAPI (DNA), CD8 (immune cells), SMA (fibroblasts)], Low-contrast images [single-channel garyscale images; DAPI (DNA), CD8 (immune cells), SMA (fibroblasts)], and Other images [single-channel garyscale images; DAPI (DNA), CD8 (immune cells), SMA (fibroblasts), along with a multichannel image].

### The goals are to quantify:
1) The number of CD8+ cells
2) The % area of tissue that is SMA+
3) Distance association of CD8+ cells and SMA+ cells, i.e., measutrement of the average dustance of CD8+ cells from nearest SMA+ cell, and the number of CD8+ cells within a given distance (20, 50, and 100 um) of SMA+ cells

### Challenges
1) Variations in the staining intenisty of SMA
2) Accurate segmentation of fibrillar, non-circular objects

The goals are to quantify: 1) The number of CD3+ cells. Note: this will look almost identical to the CD8 stain from dataset 1. 2) The number of CD3/FOXP3 double positive cells. The FOXP3 should be a stain on the same cell with a CD3+ ring. Events that are only FOXP3+ should not be counted. Cells of interest should only be all CD3+ cells, and CD3+/FOXP3+ cells. We would also like CD3+/FOXP3+ cells as a percentage of total CD3+ cells.
The folder for each dataset contains a variety of images. For each sample 3 channels are included and the file names end with either ‘DAPI’ (nuclei), ‘FITC’ (CD8), or ‘TxRed’ (SMA). The images are in greyscale, and we would like the ability to use the pipeline regardless of fluorophore for each stain. We have also included a couple powerpoint slides with examples of cells/features of interest - the file is labeled "Cell profiler info".
The goals are to quantify: 1) The number of CD3+ cells. Note: this will look almost identical to the CD8 stain from dataset 1. 2) The number of CD3/FOXP3 double positive cells. The FOXP3 should be a stain on the same cell with a CD3+ ring. Events that are only FOXP3+ should not be counted. Cells of interest should only be all CD3+ cells, and CD3+/FOXP3+ cells. We would also like CD3+/FOXP3+ cells as a percentage of total CD3+ cells.
There are two folders of images. The samples in each folder are equivalent, and are either the ‘Multichannel’ or ‘Merged’ image. In the ‘Multichannel’ folder, the FOXP3 stains are indicated by ‘Cy5’ in the file name, and the CD3 stained cells are indicated by ‘FITC’ in the file name.



