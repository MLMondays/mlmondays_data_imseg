# mlmondays_data_imseg
Datasets for ML Mondays Part 3: supervised image segmentation

## Oysternet dataset

https://scholars.duke.edu/display/pub1419444


Aerial UAV color imagery and labels of oyster reefs in shallow water, made publicly available by Duke University researcher Patrick Gray. This dataset, associated with the tool "OysterNet", consists of many small orthomosaics of intertidal oyster reefs and corresponding labels in text format.

OysterNet is described here: https://github.com/patrickcgray/oyster_net


This version of the data consists of a subset of 1000 x 1000 x 3 pixel orthomosaics of oyster reefs and corresponding labels in text (JSON) format. The dataset consists of 820 images, randomly split into 527 training images, 130 validation images, and 163 test images. Each image pixel has a 3-cm spatial resolution, so each scene is 30 x 30 m.

This dataset has only two classes: intertidal oyster reef and background. The labels have been converted from the original json format to binary label image format (where 1=reef, and 0=everything else). A tutorial describing how this was done is available here: https://colab.research.google.com/drive/1icT8sCXxEKuu_chh8uV27mnqs49ZC6VH



## OBX dataset

very high-resolution digital images of coastal environments in the Outer Banks, North Carolina. The imagery and associated label data have been curated especially for this course, as part of the USGS Remote Sensing of Coastal Change Florence Supplemental Project.

This dataset is courtesy of the U.S. Geological Survey. These data were collected as part of the USGS Remote Sensing of Coastal Change Florence Supplemental Project, and processed collectively by Wayne Wight, Jonathan Warrick (USGS-PCSMC), Christopher Sherwood (USGS-WHCMSC), Andrew Ritchie (USGS-PCSMC), Jenna Brown (USGS-MD-DE-DC WSC), Christine Kranenburg (USGS-SPCMSC), Jin-Si Over (USGS-WHCMSC), and Daniel Buscombe (USGS-PCSMC contractor). Although these data have been processed successfully on a computer system at the U.S. Geological Survey (USGS), no warranty expressed or implied is made regarding the display or utility of the data for other purposes, nor on all computer systems, nor shall the act of distribution constitute any such warranty. The USGS or the U.S. Government shall not be held liable for improper or incorrect use of the data described and/or contained herein.

The categories are (and corresponding integer values in the image labels):

* deep water (63)
* white (broke, aerated) water (128)
* shallow water and saturated ground (191)
* dry sandy terrain (255)

data/obx/sample
16 high-resolution images of

The following TFRecord format files contain 20 images and multiclass image labels each

data/obx/obx00-19.tfrec
data/obx/obx01-19.tfrec
data/obx/obx02-19.tfrec
data/obx/obx03-19.tfrec
data/obx/obx04-19.tfrec
data/obx/obx05-19.tfrec
data/obx/obx06-19.tfrec

and this one contains 7 images and multiclass image labels

data/obx/obx07-13.tfrec

The data are in random order and from different places and times.
