## Description of the purpose of each step of the image analysis pipeline along with example outputs

- [Description of the purpose of each step of the image analysis pipeline along with example outputs](#description-of-the-purpose-of-each-step-of-the-image-analysis-pipeline-along-with-example-outputs)
  - [1. RunStarDist](#1-runstardist)
  - [2. OverlayOutlines](#2-overlayoutlines)
  - [3. IdentifySecondaryObjects](#3-identifysecondaryobjects)
  - [4. IdentifyTertiaryObjects](#4-identifytertiaryobjects)
  - [5. Threshold](#5-threshold)
  - [6. Maskobjects](#6-maskobjects)


### 1. RunStarDist
Use the StarDist algorithm (https://github.com/stardist/stardist) to segment nuclei

<img src="Images/runstardist.png" width="700" height="300">


### 2. OverlayOutlines
Check the accuracy of the outlines of the nuclei segmented by RunStarDist

<img src="Images/overlayoutlines_1.png" width="700" height="300">


### 3. IdentifySecondaryObjects
Segment the whole cell outlines

<img src="Images/idsecondary.png" width="350" height="300">


### 4. IdentifyTertiaryObjects
Segment cytoplasm (whole cells minus the nuclei)

<img src="Images/idtertiary.png" width="350" height="300">


### 5. Threshold
Set the intensity threshold for deeming cells asd marker positive

<img src="Images/threshold_1.png" width="350" height="300">


### 6. Maskobjects
Keep the thresholded areas of the image using a mask and identify the cells present in those areas

<img src="Images/maskobjects_1.png" width="350" height="300">







