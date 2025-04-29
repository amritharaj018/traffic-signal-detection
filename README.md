Traffic Sign Image Classification
This project contains two parts:
1.	Traffic Sign Images  – Converts traffic sign images from PPM format to JPG format.
2.	Traffic Sign Classification Using CNN – Trains a Convolutional Neural Network (CNN) to classify traffic sign images.
________________________________________
Part 1: Traffic Sign Images 
What It Does
•	Converts all .ppm images from two input folders into .jpg format.
•	Saves the converted JPG images into separate output folders.
•	Automatically creates the output folders if they don’t exist.
•	Displays the first 10 converted images from each folder for quick visual check.
Folder Structure
•	Input folders (with .ppm images):
o	/Images/00000
o	/Images/00001
o /Images/00002
o /Images/00003
o /Images/00004
•	Output folders (where .jpg images are saved):
o	/Traffic_JPG_images/1
o	/Traffic_JPG_images/2
o	/Traffic_JPG_images/3
o	/Traffic_JPG_images/4
o	/Traffic_JPG_images/5
Requirements
•	Python 3.x
•	Libraries: Pillow, matplotlib (for image processing and display)

Part 2: Traffic Sign Classification Using CNN
What It Does
•	Loads JPG images from the /Traffic_JPG_images/ folder.
•	Resizes images to 224x224 pixels.
•	Splits the data into training (80%) and validation (20%) sets.
•	Applies data augmentation (random rotations, flipping) to training images to improve learning.
•	Builds and trains a CNN model to classify traffic signs into two categories.
•	Trains the model for 20 epochs using different optimizers (adam, adamax, rmsprop).
•	Prints and plots accuracy and loss results after training.
How To Use
1.	Convert your images to JPG using the script (Part 1).
2.	Place the JPG images in /Traffic_JPG_images/.
3.	Run the classification script.
4.	You can change the optimizer by passing a different parameter (adam, adamax, or rmsprop).
5.	You can also adjust the rotation range for augmentation (e.g., 30, 40, or 50 degrees).
Requirements
•	Python 3.x
•	TensorFlow
•	Matplotlib
•	Numpy
•	(Optional) scikit-learn for additional classification reports

Summary
This project helps you convert traffic sign images from PPM to JPG and then classify them using a CNN. The images are in a widely supported format, while the CNN model learns to identify traffic signs accurately, improving with data augmentation and different training settings.
