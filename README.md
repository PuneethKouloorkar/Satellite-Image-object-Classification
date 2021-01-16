# Satellite-Image-object-Classification

Given a Sentinel-2 satellite image, our task is to classify objects (7 classes in total) in the image. The image is labelled with integers representing different land cover objects in the image:
* 0: urban
* 1: treerow
* 2: forest
* 3: single tree
* 4: agriculture
* 5: grassland
* 6: water
* 4294967295: nodata value (leaving out from training & evaluation!)

Rasterio library of python is used to handle the image. The image has 2 bands and only the first band for training and evaluation. XG Boost is used to train the model. Further details are written in the pdf.

One can also use QGIS application to view the .tif file (satellite image) to know the number of bands in the image and other properties.
