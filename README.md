# Human Activity Recognition

#### Introduction
Smart devices have become an integral part of our day-to-day life, from smartphones to IoT devices and smartwatches. They all help our life become convenient in various aspects like fitness, time-tracking, inventory management, and productivity. To provide the services which make their usage desirable, many services feed on data. By collecting the data, the applications can improve their performance benefiting our productivity and service. In this report, we will be picking a few of the data collected from a smartphone's sensors are trying to recognize the activity being performed by the device's owner. By finding what activity the user is performing, we can find the calories burnt or sleep, count.


#### Problem Statement
In today's day and age, everyone has a smartphone, and if you did not know already, these little devices have tons of small devices, which we call sensors within them. These sensors are pretty useful for the device, especially when you are playing games. Two such sensors are an accelerometer, which measures acceleration, and a gyroscope, which measures angular velocity. These sensors collect data that can be stored and used to predict the activity the smartphone user is performing.
Using the sensor data, can we predict whether the person is walking, sitting, standing up, or laying?
Broadly speaking our task is to use the activity to map one of the important measures of how many calories have been burned through any activity performed. How many hours have you slept?
The accelerometers are often referred to as tri-axial accelerometers because they measure acceleration on X-axis, Y-axis, and Z-axis. Similarly, gyroscopes measure angular velocity in all three axes. We have time-series data for all the axes for both the measures, so in total, we have 6 time-series data as input.
And as an output, we would like to predict one of the six activities a human can perform: walking, walking upstairs, walking downstairs, sitting, standing, or laying. So, this is a multi-class classification problem.

#### Dataset
This dataset is collected from 30 persons (referred to as subjects in this dataset), performing different activities with a smartphone on their waists. The data is recorded with the help of sensors (accelerometer and Gyroscope) in that smartphone. This experiment was video recorded to label the data manually.
Accelerometer and Gyroscope readings are taken from 30 volunteers (referred to as subjects) while performing the following 6 Activities.
1. Walking
2. WalkingUpstairs
3. WalkingDownstairs
4. Standing
5. Sitting
6. Lying

Readings are divided into a window of 2.56 seconds with 50% overlapping.

Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y, and z components each. While, the gyroscope readings are the measure of angular velocities which has x,y, and z components.

Based on experts and engineers, jerk signals are calculated for BodyAcceleration readings. Fourier Transforms are made on the above time readings to obtain frequency readings. Now, on all the base signal readings., mean, max, mad, sma, arcoefficient, engerybands, entropy etc., are calculated for each window.
We get a feature vector of 561 features and these features are given in the dataset. Each window of readings is a datapoint of 561 features.
To summarize, we have presented two datasets here, one contains expert-generated features, derived by the domain experts, upon which we will be performing exploratory data analysis and building machine learning models. And the second dataset is the raw 128-dimensional time series where we will use a deep learning model.

### Read More here: [Human Activity Recognition](https://medium.com/@swapsid_/human-activity-recognition-919d8e912be6)
