# PCA-based-face-recognition Using Matlab #
## Introduction to the project
This is a very simple yet very effective face recognition system using PCA which is based on eigen values and eigen vectors. PCA basically means in a given image of size m*n, we extract only those components which are sufficient enough to represent the whole image. It is similar to the Physics concept wherein we represent a whole bode with a single point which is its center of mass. So by extracting these components, we reduce the image size remarkable and processing done after this becomes very fast. 

## Training Phase
So, first we need a database for the training phase. We select a database called face94 which has face images of many people. Each person has 20 images. So, for the training phase we select 30 person , 10 images each so the total is 300 images. This can be seen in the 'Train_Db' file. And the remaining 10 images of each person together form the Testing Phase.

## Coding in Matlab 
Now after the training folder is made, we name the images numerically 1.jpeg,2.jpeg,......300.jpeg. This helps us write the matlab code easily and training time is reduced. Now the mathematical operation on image is done in Matlab , the file for which is in the 'Train_Db' folder.Also the file is shared in the repository outside. Remember that if you are using the same code which i have shared, then make sure that the matlab file is in the 'Train_Db' folder. 

## Testing Phase.
After your training is done, we create the testing folder named 'testing_db1' mentioned above. The folder is also shared in the repository. In the testing phase, we write matlab code such that it prompts the user to select an image from the testing folder, and then the distance of that image is taken from each images in the training set. The image which has the least distance with the query image is the reccognized image and it is given as the output. 
The best part about this project is that it helps to recognize distorted images with maximum accuracy!

## Use of filters
Sometimes images contains noise, some editing, lighting condition changes,etc. This can affect the recognization of that image. So in such cases, we can use filters like mean filter, median filter, homomorphic filter, etc which helps to get a clearer image sufficient enough to be recognized.

## Further uses of PCA
This kind of PCA based recognition system can be used not only to recognize faces, but also other things like handwriting, animal species, audio,etc.
