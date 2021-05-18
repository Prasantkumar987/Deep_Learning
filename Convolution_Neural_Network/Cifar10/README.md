# Cifar10 
The CIFAR-10 dataset (Canadian Institute For Advanced Research) is a collection of images that are commonly used to train machine learning and computer vision algorithms. It is one of the most widely used datasets for machine learning research.<br>
The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.<br>
<br>
The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.<br>

Here I built a classifier using Convolutional Neural Network to classify images of **10 classes** of images got accuracy on training set **0.7653** and validation accuracy **0.7252**.<br>
You can take help of Cifar10.ipynb file where I coded it in this folder.<br>

### Parameters:
Input size of Image = (32,32,3) (Here 3 denotes RGB, three colors)<br>
Activation function in Conv2D = relu<br>
Number of Convolutional layers = 3<br>
Number of Pooling layers = 2<br>
Number of hidden layers = 2<br>
Activation function in Dense layers= relu and gelu<br>
Number of neurons = 256<br>
optimizer = Adamax<br>
loss = SparseCategoricalCrossentropy<br>
metrics = accuracy<br>
epochs = 20<br>

I got accuracy on validation data of **0.7252** .It took me about 2-3 mins to train it as dataset is also very large. Generally it takes time and it also depends on your computional power.<br>
![accuracy](https://user-images.githubusercontent.com/54981696/118615448-616ba780-b7de-11eb-817b-73fa6503d8c9.png)

  
### Tring model on some other images
After getting accuracy of **0.7252**, I used it on some images which I took from [Upslash](unsplash.com) and tested them on model, it gave perfect results on them.<br>

### You should also try it out. 
