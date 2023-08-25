# Customer Age Estimation for a Supermarket Using Computer Vision
The network supermarket "Bread-Salt" is implementing a computer vision system for processing customer photographs. Photo capture in the checkout area will help determine the age of customers in order to:

- Analyze purchases and suggest products that might interest customers in that age group.
- Monitor the honesty of cashiers when selling alcohol.
This project involves building a model that estimates the approximate age of a person from a photograph. The dataset consists of people's photographs with their corresponding ages provided.

## Project Execution Instructions
The project involves the following steps:

- Conduct exploratory analysis of the photograph dataset.
- Prepare the data for training.
- Train a neural network and assess its quality.

## Exploratory Data Analysis
The exploratory analysis of the photograph dataset revealed the following insights:

- The dataset contains 7591 photographs along with the corresponding ages of individuals.
- The age distribution shows spikes at milestone ages, suggesting potential rounding during labeling.
- The photographs depict people of different genders, ages, nationalities, and angles.
## Data Preparation
To prepare the data for training, the following steps were taken:

 - The data was loaded using the ImageDataGenerator with augmentations such as horizontal and vertical reflections, rotations, and shifts applied.
 - The dataset was divided into training and validation sets.
## Model Training
The model was trained using the following approach:

 - A ResNet50 backbone pre-trained on ImageNet was used.
 - A neural network was built on top of the backbone with a Global Average Pooling layer and a Dense output layer.
 - The model was compiled using the Mean Squared Error (MSE) loss and Mean Absolute Error (MAE) metric.
 - The training was carried out over multiple epochs with increasing accuracy.
## Analysis of the Trained Model
The trained model demonstrated the ability to estimate the age of individuals from photographs with good accuracy. The Mean Absolute Error (MAE) on the test set decreased with each epoch and eventually reached 7.4438, which meets the project's requirement of not exceeding 8.

## Conclusion
This project successfully developed a computer vision model for estimating the age of individuals from their photographs. The model can be deployed in the network supermarket "Bread-Salt" to analyze customer ages and provide relevant recommendations for targeted product suggestions and monitoring cashier honesty during alcohol sales. The achieved MAE on the test set demonstrates the model's effectiveness in estimating customer ages.




