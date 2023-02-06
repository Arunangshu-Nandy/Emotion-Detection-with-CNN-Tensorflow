In this case I take the dataset from Kaggle for facial emotion detection. I explore the sample data images along with associated class names.
In the next step we access the data directory and create a small dictionary with 0-7 numbers for each of facial expressions. I also create another dictionary with path against each of the expressions.
I create input (X) & output (y) numpy array for the dataset.
After scaling the image  (dividing the numpy array by 255), I feed the same to our CNN model(with padding). In CNN I have kept 3 layers along with one Maxpooling layer for each layer.
I trained the model for 5 epochs and found the accuracy to be 51%. However while I used the same model for prediction I received accuracy of 47%. 
I also use data augmentation technique to experiment on the accuracy of the model
After the same model with 5 epochs the accuracy is 38% (lower than initial one) and prediction accuracy is 24% (also very low).
In order to increase the accuracy we need to change the hyper-parameters and increase number of epochs.

Data Source-https://www.kaggle.com/datasets/ananthu017/emotion-detection-fer

Techniques used- Tensorflow, CNN, Data Augmentation, 
