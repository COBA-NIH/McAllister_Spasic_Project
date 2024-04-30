### This repository contains the pipelines developed for quantifying and determining spatial relationships bteween subtypes of immune cells and fibroblasts in tissues stained using multiplex immunofluorescence technology

# 1. Project outline

## 1.1. Dataset 1:
The dataset comprises three-channel images - DAPI (DNA), FITC (CD8+ T-cell), Texas Red (SMA+ fibroblasts). Images were received in three sets; high-contrast images, low-contrast images, and other images (composite/merged images).

### 1.1.1. Objectives:
1) Count the number of CD8+ cells
2) Measure the percentage of tissue area that is SMA+
3) Determine spatial relationship between CD8+ cells and SMA+ areas, i.e., measure the average distances of CD8+ cells from nearest SMA+ areas, and the number of CD8+ cells within a given distance (20, 50, 100, and 200 um) of the SMA+ areas

### 1.1.2. Challenges
1) Variable intensity of SMA-expression in the fibroblasts
2) Accurate segmentation of fibroblasts (fibrillar, elongated, non-circular cells)
3) Accurate segmentation of clumped nuclei

## 1.2. Dataset 2:
This dataset comprises three-channel images - DAPI (DNA), FITC (CD3+ T-cells), Cy5 (FOXP3+ T-cells).

### 1.2.1. Objectives:
1) Count the number of CD3+ cells
2) Count the number of CD3-FOXP3 double-positive cells and percentage of CD3+ cells that are CD3-FOXP3 double-positive

### 1.2.2. Additional objectives
 - Ability to use the pipeline regardless of fluorophore for each stain

# 2. Files in this repository:

## 1. Pipelines

### (i) Pipelines for Dataset 1
A. CellProfiler pipeline without plugins: CD8-SMA-tumor_CellProfiler.cpproj; CD8-SMA-tumor_CellProfiler.cppipe
B. CellProfiler pipeline with RunStarDist plugin: CD8-SMA-tumor_RunStarDist.cpproj; CD8-SMA-tumor_RunStarDist.cppipe

### (ii) Pipelines for Dataset 2
A. CellProfiler pipeline without plugins: CD3-FoxP3-tumor_CellProfiler.cpproj; CD3-FoxP3-tumor_CellProfiler.cppipe
B. CellProfiler pipeline with RunStarDist plugin: CD3-FoxP3-tumor_RunStarDist.cpproj; CD3-FoxP3-tumor_RunStarDist.cppipe

## 2. Description of all the steps with example images are provided for both pipelines
