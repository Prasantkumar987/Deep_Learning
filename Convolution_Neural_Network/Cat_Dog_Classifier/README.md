# Cat-Dog Classifier (using CNN)

Here I built a classifier using Convolutional Neural Network to classify images of **Cat and Dog**.<br>
I used the dataset for this kaggle and you can use it by clicking [Here](https://www.kaggle.com/prasantdixit/cat-dog-cnn/data).<br>
You can take help of Cat-Dog-CNN.ipynb file where I coded it in this folder.<br>

### Parameters:
Input size of Image = (64,64,3) (Here 3 denotes RGB, three colors)<br>
Activation function in Conv2D = relu<br>
Number of Convolutional layers = 2<br>
Number of hidden layers = 1<br>
Activation function in Dense layers= relu<br>
Number of neurons = 100<br>
optimizer = Adamax<br>
loss = binary_crossentropy<br>
metrics = accuracy<br>
epochs = 10<br>

I got accuracy on validation data of **0.7914** .It took me about 10 mins to train it as dataset is also very large. Generally it takes time and it also depends on your computional power.<br>
![Screenshot (283)](https://user-images.githubusercontent.com/54981696/118532065-2dec3700-b764-11eb-86d8-3a514cfa8cf3.png)
![Screenshot (284)](https://user-images.githubusercontent.com/54981696/118532106-347aae80-b764-11eb-8b9e-9908b0ba757a.png)


  
### Tring model on some other images
After getting accuracy of **0.7914**, I used it on some images which I took from [Upslash](unsplash.com) and tested them on model, it gave perfect results on them.<br>

### You should also try it out. 
