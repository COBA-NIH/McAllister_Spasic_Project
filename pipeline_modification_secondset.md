### Pipeline modification for second set of images received Jan 2024

For the second set of images, the challenge is addressing the variability in staining quality in identifying SMA-positive cells, getting rid of false-positive areas, and identifying SMA-positive cells (fibroblasts) which are elongated in shape.
below are some example images indicating the performance of the pipeline on the second set of images.
Pipeline was run on 42 image sets (126 images)

#### I. Primary, secondary, and tertiary object identification seem to be working fine / requiring minor modifications

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/862f9ec7-84cd-48e2-8d58-722c8ad0a861)


![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/2aaea43e-4dd8-4836-95d9-e9944c4d5f97)


![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/0468f242-ee7c-409c-9fe0-5e24061dc1d8)


#### II. CD8-positive cell identification seem to be working fine / requiring minor modifications

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/b75fe0a3-9401-4a52-94eb-2428a14d23bf)


#### III. Original pipeline is picking up some false-positive signals

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/136db19c-9d95-43ba-8906-0328827e11d5)


#### IV. Examples of identifying SMA-positive areas after modifying outlier fractions, deviations, and variance methods

Some of the false-negative cells can be filtered out but this is filtering out some weakly-stained parts of the fibroblasts (elongated cells)

![image](https://github.com/COBA-NIH/McAllister_Spasic_C-S-Project/assets/139376717/4dad12fc-322f-4a9b-a600-aa894b6a9bd5)



















