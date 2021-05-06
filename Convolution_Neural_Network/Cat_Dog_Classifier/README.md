# Cat-Dog Classifier (using CNN)

Here I built a classifier using Convolutional Neural Network to classify images of **Cat and Dog**.<br>
I used the dataset for this kaggle and you can use it by clicking [Here](https://www.kaggle.com/prasantdixit/cat-dog-cnn/data).<br>
You can take help of Cat-Dog-CNN.ipynb file where I coded it in this folder.<br>

## Steps
### Importing Dataset
Here to make convolutional model, we use images as our data. Images datasets are generally too large(expected in few 100 MBs) can't be accessed be excessed by uploading it into our notebook. Because of which we import it using directory in which it is present  using a Keras class **ImageDataGenerataor** and also preprocess of train and test data using it.<br>

### Building CNN Model
There are few steps which I have followed to build CNN model which are following:<br>
1.Adding **Convolution layers**<br>
2.Adding Pooling(particularly **Max Pooling**)<br>
3.**Flattening** the output from previous layers(converting 3-D array to 1-D array)<br>
4.for **Full Connection** adding Dense layers<br>
5.**Output Layer**(It classfies the Image into Cat or Dog)<br>

### Training Model
1.Compile the model on optimizer, loss, and metrics<br>
Before fiting our trianing data into model, we have to compile our model from best paramters for data to get best results out of it.<br>
  I used **Adam** optimizer because it worked best for this dataset.<br>
  I used **binary_crossentropy** for loss because here we have only classes, so this loss function is best to deal with it.<br>
  I used **accuracy** for metrics parameter.<br>
2.Fiting data and training model on dataset<br>
  Here I fitted my data on model and used by testing data for validating the model.<br>
  I tried 30 epoches train this model and got accuracy on validation data of **0.8072** .It took me about 10 mins to train it as dataset is also very large. Generally it takes time and it also depends on your computional power.<br>
  
### Tring model on some other images
After getting accuracy of **0.8072**, I used it on some images which I took from [Upslash](unsplash.com) and test on them, it gave perfect results for me.<br>

### You should also try it out. 
