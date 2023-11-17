# Description of the pipeline modification

#### The previously created 'IF Red Blue 8 well slides' pipeline was modified to incorporate some of the additional functionalities available in CellProfiler 4.2.6. Ideally the pipeline should be run in CellProfiler 4.2.6, but should work on CellProfiler 4.2.5 as well. A description of the modules that current pipeline comprises is provided below along with the results of running the image analysis modules on example images chosen from the high-contrast, low-contrast, and other image sets.

I. The metadata and names and types modules were changed to extract sample IDs and and channel names from the image file names


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/863b3725-a646-4ef7-92b1-cdde358fc7c0)

![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/ad1c03a2-cd1c-4376-aa9f-6e27616d42d4)



II. IdentifyPrimaryObject module was modified to ensure accurate segmentation of the variably sized nuclei and discrete as well as the clumped nuclei from the high-contrast, low-contrast, and other images


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/7cb391ac-699d-4ba5-aee1-16139cf51e02)


A. Example from high-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/7619e78d-8697-4948-a8c1-3332a64120a1)


B. Example from low-contrast image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/0118e47c-0c90-43d9-9303-3ffde5f4a33b)


C. Example from other image


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/06c36c79-b966-490a-9e93-ced0bb327dc7)


III. IdentifySecondaryObject module was modified to identify the cell boundaries in the CD8 single channel images using Distance-N method, as there were no cytoplasmic stain available


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/01a35775-6a48-45a1-a298-bf4d3a84267c)



IV. IdentifyTertiaryObject module was used to identify cytoplasm of the cells


![image](https://github.com/COBA-NIH/McAllister_Spasic_CD8-SMA-tumors/assets/139376717/74286605-e156-445c-8a93-eb7d5f11de8b)



V. Identifying CD8-positive cells: 





















