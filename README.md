# Tensorflow-Tree-Cover-Classification

## Introduction

As a way to continue working with Tensorflow/Keras and neural networks, I found this dataset from the US Forest Serivice about forest cover based off cartographic variables. 

The goal of the project is to use neural networks to predict the type of forest cover we can expect based off inputs such as elevation, slope, aspect, etc..


## Dataset

US Forest Service - GeoData - Tree Cover Canopy Dataset

https://data.fs.usda.gov/geodata/rastergateway/treecanopycover/

The datasets include four wilderness areas located in the Roosevelt National Forest of Northern Colorado. The areas represent forests with minimal human-caused disturbances, so existing forest cover types are mainly a result of ecological processes rather than human forest management practices.

## Model

We used a Sequential model with 4 hidden layers, and used Sparse Categorical Crossentropy to measure our loss.

The model was kept with around ~5,000 to keep runtime low. 

## Conclusion

The model we created had close to a 90% accuracy, and had a relatively high precision, recall, and F1 score (all in the 80%+ range). Some things to note were:
- the data *may have been biased* towards certain forest cover types 
