# 425-AI-project
Project for CSC425 that uses AI to identify/classify images
got dataset for Kaggle of images of a four suit of playing cards
link for dataset:
https://www.kaggle.com/datasets/gpiosenka/cards-image-datasetclassification?select=train 

This dataset features a training, testing and valid dataset. Within each are folder of card images with each folder being a different playing card. For example there is a folder dedicated to the ace of spades images. The training has around 7500 entries with valid and test having around 250. 

For processing the data, it is processed with tensorflow keras image_dataset_from_directory. The code uses the google drive directory to get the dataset file. 

They are then concatenated and lattened into X_train/test and y_train/test for using them in the model. 

The models used for image classification are SVM:Linear,SVM:RBF and MLPclassification. The results of the prediction are held within accuracy score. 

Then they are put into a table to read the results and deafferenting combinations of entries loaded,execution times and image quality are shown with the table.
10,50 and 100 entries are shown
128x128 and 256x256 image quality are shown
