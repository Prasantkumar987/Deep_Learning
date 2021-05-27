# NewYork Stock Exchange Price Prediction

![Screenshot (286)](https://user-images.githubusercontent.com/54981696/119790161-53f6a180-bef1-11eb-8a7a-00bc9d698722.png)
####You can see my accuracy, validation accuracy, loss, validation loss, epochs [HERE](https://wandb.ai/prasantdixit/NewYork%20Stock%20Price%20Prediction-%20V2/reports/NewYork-Stock-Exchange-Price-Prediction-- Vmlldzo3MzA0ODE)

## 1. Problem Statement
Historical data of NewYork Stock Exchange for various companies are given, chose some of them and Predict their future Prices using given Prices. I chose 5 MNCs named Apple, ADM, Amazon, Google, IBM and tried to predict their future prices.

I predicted Stock prices of these companies with *Accuracy on test dataset of* **95%**.

![Stock_price](https://user-images.githubusercontent.com/54981696/119793756-7f2ec000-bef4-11eb-9cd5-4684361448f0.png)


## 2. Model
**Parameters:**
1. Activation function : tanh and linear
2. batch size : 32
3. Dropout : 0.2
4. Epochs : 200
5. Hidden layer 1 : 128
6. Hidden layer 2 : 128
7. Hidden layer 3 : 32
8. Loss : Mean squared error
9. Metrics : accuracy

#### Loss and Accuracy
At Epoch 1:
1. loss: 0.6609
2. accuracy: 0.2593 
3. val_loss: 0.0542 
4. val_accuracy: 0.2035

At Epoch 50:
1. loss: 0.0036 
2. accuracy: 0.8804 
3. val_loss: 5.7430e-04 
4. val_accuracy: 0.9314

At Epoch 100:
1. loss: 0.0034 
2. accuracy: 0.8852 
3. val_loss: 4.6275e-04 
4. val_accuracy: 0.9362

At Epoch 150:
1. loss: 0.0035 
2. accuracy: 0.8745 
3. val_loss: 3.3246e-04 
4. val_accuracy: 0.9330

At Epoch 200:
1. loss: 0.0032 
2. accuracy: 0.8723 
3. val_loss: 2.5394e-04 
4. val_accuracy: 0.9518

![Accuracy_and_LossVSEpochs](https://user-images.githubusercontent.com/54981696/119793847-966dad80-bef4-11eb-8967-4551ccc8b45e.png)

# 3. How to use it?
1. First of all you need to download resultant_model.h5 file.
2. After that you need to import tensorflow and keras
3. Then you need to load model using keras.models.load_model()
4. After loading model you can predict your values.

#Importing the libraries
import tensorflow as tf
from tensorflow import keras

#Loding the model
loded_model = keras.models.load_model('file_path/stock_predict_1.h5')

#Predicting the values
loded_model.predict("Any value you want to predict")

# 4. Actual and Predicted values
![PriceVSCompany](https://user-images.githubusercontent.com/54981696/119794255-ff552580-bef4-11eb-8ce0-918ff6a3d145.png)

# 5. GPU Usage
![Screenshot (287)](https://user-images.githubusercontent.com/54981696/119794394-214ea800-bef5-11eb-944d-8257e1ae1bc1.png)

# 6. Credits
I would like to thank to my friend [Rahul](https://github.com/RAHUL-KAD) for telling me about Weights and Biases and many other Kernel writter on [Kaggle](kaggle.com) for helping me build this project.


