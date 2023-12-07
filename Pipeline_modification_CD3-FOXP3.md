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


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/01a35775-6a48-45a1-a298-bf4d3a84267c)



#### IV. IdentifyTertiaryObject module was used to identify cytoplasm of the cells


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/74286605-e156-445c-8a93-eb7d5f11de8b)



V. Identifying CD8-positive cells: Thresholding module was applied to identify CD8-positive cells and the MaskObjects module was used to only retain the CD8-positive cells and exclude the remaining areas. Accuracy of CD8-positive cell identifcation was examined by overlaying outlines of the masks on the single-channel CD8-image using OverlayOutlines


A. Example from high-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/f710ef51-98bb-467d-8b9f-6c904233fd38)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/cef1f855-3f59-4c57-b08b-db2049100288)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/1dbc28dd-eb0e-4f0f-ad5c-71f4050be9c5)


B. Example from a low-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/74e976e7-79e5-4d52-bb68-e656f66b7dfd)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/95c6d3e4-926a-42d6-8e41-4e1164c0a1db)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/fc31b086-152f-47df-bb0e-f75aec75d1c4)



VI. Measuring SMA-positive areas: Thresholding module was applied to identify SMA-positive areas and the MaskObjects module was used to only retain the SMA-positive areas. Accuracy was examined as examined by overlaying outlines of the masks on the single-channel SMA-images using OverlayOutlines.


A. Example from high-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/06c61360-f7a6-406c-8599-3ee1a6ed2194)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/979dd96a-9ca0-429b-8bb0-2a39bef6968a)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/02b818e9-24aa-4f25-bce3-00cf9631c646)



B. Example from a low-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/bbb23557-062e-445c-bfd6-bcabb22d38ef)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/1b64a3c9-2b28-401f-92ec-f885d0ae6685)


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/3aecb25e-b081-447e-b205-31b0fa619a5f)



VIII. Finally, the following modules were added to address the research questions for this study:
  (i) MeasureImageAreaOccupied: To measure SMA-positive tissue area
  (ii) MeasureObjectNeighbours: To measure SMA-positive areas within 20u, 50u, and 100u from CD8-positive cells
  (iii) DistanceTransform: For more detailed neighborhood analyses for CD8-positive cells
























