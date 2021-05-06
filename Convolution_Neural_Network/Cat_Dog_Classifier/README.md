# Cat dog classifier

Here I built a classifier using Convolutional Neural Network to classify images of **Cat and Dog**.
I used the dataset for this kaggle and you can use it by clicking [Here](https://www.kaggle.com/prasantdixit/cat-dog-cnn/data).
You can take help of Cat-Dog-CNN.ipynb file where I coded it in this folder.

## Steps
### Importing Dataset
Here to make convolutional model, we use images as our data. Images datasets are generally too large(expected in few 100 MBs) can't be accessed be excessed by uploading it into our notebook. Because of which we import it using directory in which it is present  using a Keras class **ImageDataGenerataor** and also preprocess of train and test data using it.

### Building CNN Model
There are few steps which I have followed to build CNN model which are following:
1.Adding **Convolution layers
2.Adding Pooling(particularly **Max Pooling**)
3.**Flattening** the output from previous layers(converting 3-D array to 1-D array)
4.for **Full Connection** adding Dense layers
5.**Output Layer**(It classfies the Image into Cat or Dog)

### Training Model
1.Compile the model on optimizer, loss, and metrics
Before fiting our trianing data into model, we have to compile our model from best paramters for data to get best results out of it.
  I used **Adam** optimizer because it worked best for this dataset.
  I used **binary_crossentropy** for loss because here we have only classes, so this loss function is best to deal with it.
  I used **accuracy** for metrics parameter.
2.Fiting data and training model on dataset
  Here I fitted my data on model and used by testing data for validating the model.
  I tried 30 epoches train this model and got accuracy on validation data of **0.8072** .It took me about 10 mins to train it as dataset is also very large. Generally it takes time and it also depends on your computional power.
  
### Tring model on some other images
After getting accuracy of **0.8072**, I used it on some images which I took from [Upslash](unsplash.com) and test on them, it gave perfect results.
