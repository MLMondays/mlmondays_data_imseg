# mlmondays_data_imseg
Datasets for ML Mondays Part 3: supervised image segmentation

## Oysternet dataset

https://scholars.duke.edu/display/pub1419444


Aerial UAV color imagery and labels of oyster reefs in shallow water, made publicly available by Duke University researcher Patrick Gray. This dataset, associated with the tool "OysterNet", consists of many small orthomosaics of intertidal oyster reefs and corresponding labels in text format.

OysterNet is described here: https://github.com/patrickcgray/oyster_net


This version of the data consists of a subset of 1000 x 1000 x 3 pixel orthomosaics of oyster reefs and corresponding labels in text (JSON) format. The dataset consists of 820 images, randomly split into 527 training images, 130 validation images, and 163 test images. Each image pixel has a 3-cm spatial resolution, so each scene is 30 x 30 m.

This dataset has only two classes: intertidal oyster reef and background. The labels have been converted from the original json format to binary label image format (where 1=reef, and 0=everything else). A tutorial describing how this was done is available here: https://colab.research.google.com/drive/1icT8sCXxEKuu_chh8uV27mnqs49ZC6VH
