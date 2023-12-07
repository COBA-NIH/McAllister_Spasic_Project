# Description of the pipeline modification

### The previously created 'IF Red Green Blue images' pipeline was modified to incorporate some of the additional functionalities available in CellProfiler 4.2.6. Ideally the pipeline should be run in CellProfiler 4.2.6, but should work on CellProfiler 4.2.5 as well. A description of the modules that current pipeline comprises is provided below along with the results of running the image analysis modules on example images chosen from the high-contrast, low-contrast, and other image sets.


#### I. The metadata and names and types modules were changed to extract sample IDs and and channel names from the image file names

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/2046ec8e-620d-4d23-a7c9-dacd294003bf)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/7ea0fef2-3ab2-4fc6-9be2-0a32fe7c8913)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/952f1a75-ef96-4ef8-9224-7ce4fc8dcdec)


#### II. IdentifyPrimaryObject module was modified to ensure accurate segmentation of the variably sized nuclei and discrete as well as the clumped nuclei

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/e8f3d223-8155-4d04-8c03-c651b793ad51)


Example (image set 1)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/d2419e67-b11f-4695-a368-159e0a0c88d3)

Example (image set 2)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/5b4aa4e1-dd23-4110-bc0e-307256509fbd)


#### III. IdentifySecondaryObject module was modified to identify the cell boundaries using Distance-N method, as there were no cytoplasmic stain available


![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/4c8b441d-7dba-4e87-b384-2f54a6806d88)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/b295e111-995c-4e4b-ace2-9831ab42f8b8)


#### IV. IdentifyTertiaryObject module was used to identify cytoplasm of the cells


![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/8c44554c-47dc-42b9-8f32-aa0ed537c418)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/cd81dfed-fce0-4a4c-80f3-245a6460b091)



#### V. Identifying CD3-positive cells: Thresholding module was applied to identify CD8-positive cells and the MaskObjects module was used to only retain the CD8-positive cells and exclude the remaining areas. Accuracy of CD8-positive cell identifcation was examined by overlaying outlines of the masks on the single-channel CD8-image using OverlayOutlines








#### VI. Identifying FOXP3-positive cells: Thresholding module was applied to identify CD8-positive cells and the MaskObjects module was used to only retain the CD8-positive cells and exclude the remaining areas. Accuracy of CD8-positive cell identifcation was examined by overlaying outlines of the masks on the single-channel CD8-image using OverlayOutlines





#### VII. Finally, the following modules were added to measure marker intensities and double-positive (CD3pos-FOXP3pos) cells:
  (i) MeasureImageAreaOccupied: To measure SMA-positive tissue area
  (ii) MeasureObjectNeighbours: To measure SMA-positive areas within 20u, 50u, and 100u from CD8-positive cells
  (iii) DistanceTransform: For more detailed neighborhood analyses for CD8-positive cells





