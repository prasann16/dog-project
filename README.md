[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

In this project, I built a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, the algorithm identifies an estimate of the canine’s breed.  If supplied an image of a human, the code identifies the resembling dog breed.

![Sample Output][image1]

## Implementation
The model was built using Convolutional Neural Networks (CNN) in Keras. Training of the NN layers was first attempted from scratch which did not produce good results. Trasfer learning was then used and model was trained on top of pretrained layers from Resnet-50 model. The final mode acheived more than 80% accracy. 

All the code is in the Jupyter Notebook.

## Data

1. [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

2. [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

3. Pretrained model: [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.
