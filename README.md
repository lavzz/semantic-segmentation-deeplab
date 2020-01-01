# semantic-segmentation-deeplab

This repo is a helpful reconstruction of the keras implementation of deeplabv3 created by github user @bonlime tailored for doing off-the-shelf inference using pre-trained mobilenet or xception net 

Google's deeplab is the latest state of the art in semantic segmentation and combines the elements of previously discovered technologies like fully convolutional nets, encoder-decoder framework and dilated convolutions to create a very deep and very accurate network that works across many different applications 

Google's original implementation of deeplab is available here -> https://github.com/tensorflow/models/tree/master/research/deeplab 

Google's implementation is difficult for beginners to follow along and its written mainly in tensorflow , not keras 

Overtime, I will be adding more complexity to this repo and include scripts for training on custom datasets, transfer learning, fine-tuning etc. 

A really good explanation of dilated convolutions and deeplab's structure is explained here https://towardsdatascience.com/review-deeplabv3-atrous-convolution-semantic-segmentation-6d818bfd1d74


USAGE 
I created a notebook called 'off-the-shelf' inference with some helpful comments ...it will be the best way to get started if you want to play with this and understand what is going on 

Step by Step 
#1 Download/clone the repo
#from the command line 
git clone https://github.com/lavzz/semantic-segmentation-deeplab.git

#2 cd into semantic-segmentation-deeplab 
cd semantic-segmentation-deeplab 

#3 open up requirements.txt to make sure you are on the right versions for various libraries. if not, install them using pip or sudo. In particular, this only works with tensorflow 2.0. One way to check your tensorflow version from the command line is - 
python import tensorflow as tf
print(tf.__version__)

if you get anything other than 2.0.0, you are on the wrong version and will need to update 

#4 from the command line or via anaconda navigator, start jupyter notebook and open 'off-the-shelf-inference.ipynb'. follow the steps there to recreate inference on your own images by uploading them to the /imgs folder 

Since we are playing only with pre-trained models, GPUs are not needed to run this 



