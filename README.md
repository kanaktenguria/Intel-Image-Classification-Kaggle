-----------------------------------------READ ME-------------------------------------------

Author: Kanak Tenguria


Dataset Kaggle Link: https://www.kaggle.com/puneet6060/intel-image-classification
---------------------------------------Requirements:---------------------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Python Version: 3.6
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Packages:
matplotlib==3.3.3
numpy==1.18.5
scikit-learn==0.23.2
tensorflow==2.3.1
h5py==2.10.0
pyyaml==5.3.1
pickle
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Above mentioned packages are required to run the project.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Submitted zip includes 3 python files. One is for CNN Model (cnnproject2.py), one for ANN Model (annproject2.py) and lastly for Random Forest Model (randomforestproject2.py). 

Data is submitted in the form of pickle files and can be found in the DataFiles directory.

DataFiles Directory contains 7 files:
X_train.pck and y_train.pck -> Used for training
X_valid.pck and y_valid.pck -> Used for validation after every epoch 
X_test.pck and y_test.pck -> Used for testing
pred_image.pck -> Unlabelled data used for testing model performance manually by humans

Saved weights for the best performing trained model can be found in the directories CNN_Model, ANN_Model and RandomForest_Model where the name of the directory indicates which model the weights belong to.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-------------------------------More info on the python files:------------------------------

Code for training and testing of the respective models are included in all the files. All the training code is commented out 
and if you run the code right away, it will load saved weights and predict label for 9 random images
from unlabelled dataset (pred_image.pck). All the images and predicted labels will be displayed to 
the user to verify the performance manually. Along with this, it will also predict accuracy, confusion matrix 
and classification report of model on test dataset (X_test.pck and y_test.pck) and print it on the console.

If you uncomment the training code, it will start training the model and save the weights at specified path after "each epoch" for ANN and CNN models. I recommend to change the paths otherwise it will overwrite my already saved weights. For random forest, it will save the weights after the training is over.

For ANN and CNN, once the training is finished, it will plot two graphs, training accuracy v/s validation accuracy and training loss v/s validation loss.

Comments are provided in the python files as well for better understanding.
