# Cifar10 
The CIFAR-10 dataset (Canadian Institute For Advanced Research) is a collection of images that are commonly used to train machine learning and computer vision algorithms. It is one of the most widely used datasets for machine learning research.<br>
The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.<br>
<br>
The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.<br>
## Steps
### Importing Dataset
Cifar-10 dataset is already installed in datasets class of keras. I imported them using tensorflow and keras class datasets. After importing dataset, scaled pixels of images between 0 and 1<br>

### Building CNN Model
There are few steps which I have followed to build CNN model which are following:<br>
1.Adding **Convolution layers**<br>
2.Adding Pooling(particularly **Max Pooling**)<br>
I made interconnection between the Covolutional layers and Pooling layers to improve network results.
4.**Flattening** the output from previous layers(converting 3-D array to 1-D array)<br>
5.for **Full Connection** added 2 Dense layers<br>
6.**Output Layer**(It classfies the Image into 10 classes of cifar-10)<br>

### Training Model
1.Compiled the model using best optimizer, loss, and metrics for the cifar-10 dataset <br>
Before fiting our training data into model, we have to compile our model from best paramters for data to get best results out of it.<br>
  I used **Adam** optimizer because it worked best for this dataset.<br>
  I used **SparseCategoricalCrossentropy** function for minimizing loss because here we have 10 classes of images, so this loss function fits best to deal with it.<br>
  I used **accuracy** for metrics parameter.<br>
2.Fiting data and training model on training dataset and testing it on test dataset<br>
  Here I fitted my training data on model and used by testing data for validating the model.<br>
  I tried 10 epoches to train this model and got accuracy on validation data of **0.6867** .It took me about 5 mins to train it as dataset is also very large. Generally it takes time and it also depends on your computional power and number of images also.<br>
  
### Tring model on some other images
After getting accuracy of **0.6867**, I used it on some images which I took from [Upslash](unsplash.com) and tested them on model.
Very firstly,I gave an image of Dog which is
![image](https://user-images.githubusercontent.com/54981696/117552002-8afe3380-b066-11eb-899c-fad1c0b57c3e.png)
and got results as horse. <br>
After that I tried another image of Dog which is
![image](https://user-images.githubusercontent.com/54981696/117552165-74a4a780-b067-11eb-93e2-606f25f9e323.png)
### You should also try it out. 


