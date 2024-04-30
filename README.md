### This repository contains the pipelines developed for quantifying and determining spatial relationships bteween subtypes of immune cells and fibroblasts in tissues stained using multiplex immunofluorescence technology

# Project outline

## Dataset 1:
The dataset comprises three-channel images - DAPI (DNA), FITC (CD8+ T-cell), Texas Red (SMA+ fibroblasts). Images were received in three sets; high-contrast images, low-contrast images, and other images (composite/merged images).

### Objectives:
1) Count the number of CD8+ cells
2) Measure the percentage of tissue area that is SMA+
3) Determine spatial relationship between CD8+ cells and SMA+ areas, i.e., measure the average distances of CD8+ cells from nearest SMA+ areas, and the number of CD8+ cells within a given distance (20, 50, 100, and 200 um) of the SMA+ areas

### Challenges
1) Variable intensity of SMA-expression in the fibroblasts
2) Accurate segmentation of fibroblasts (fibrillar, elongated, non-circular cells)
3) Accurate segmentation of clumped nuclei

## Dataset 2:
This dataset comprises three-channel images - DAPI (DNA), FITC (CD3+ T-cells), Cy5 (FOXP3+ T-cells).

### Objectives:
1) Count the number of CD3+ cells
2) Count the number of CD3-FOXP3 double-positive cells and percentage of CD3+ cells that are CD3-FOXP3 double-positive

### Additional objectives
 - Ability to use the pipeline regardless of fluorophore for each stain

## Files in this repository:

1. 