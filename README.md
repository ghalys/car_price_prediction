# car_price_prediction
In this project, we try to predict the price of cars from images and we compare different technics like classification and regression.

for this, we use a dataset of car images provided by kaggle in https://www.kaggle.com/datasets/eduardo4jesus/stanford-cars-dataset
We also provide code to detect the car coordinates with Yolo.
![image](https://github.com/ghalys/VCE_03/assets/127297865/1a963930-4697-4f58-a17c-aebd0c4073ce)

After the classification, we try different options to select the predicted price, considering sometimes classes that has a confidence above a threshold.

## Vgg 16
![image](https://github.com/ghalys/VCE_03/assets/127297865/5086c6b2-a9fa-4130-9cb9-9185fbec6470)
### accuracy of 90%

## ResNet 50
![image](https://github.com/ghalys/VCE_03/assets/127297865/0c1129e5-ff0b-43b2-b9fc-45914757c389)
### accuracy of 94%

After analysis of the prices over our testing dataset, depending on the distance chosen, we can consider either classes with a confidence that exceed a threshold of 20% or simply select the class with the highest confidence.
![image](https://github.com/ghalys/VCE_03/assets/127297865/15d0c791-13ef-4721-8de0-54cec062ff56)

# 2) Regression with ResNet 50
We also tried to predict the price directly from the images using ResNet adapted to the regression. However, we obtain less interesting results. We did not pass a lot of time on this approach so more improvement can be made.
![image](https://github.com/ghalys/car_price_prediction/assets/127297865/1e940ec2-27ff-4631-b69e-c542faaef81b)


# 3) Classification with Yolo Features
We devided prices into 15 categories and used features that were extracted from Yolo model. We got an accuracy of 20%.
