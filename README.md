# Face-recognition-based-attendance-system

This project records the attendance of the student based on face recognition captured using web camera. Face recognition, encoding and matching is done using dlib and opencv.

Face recognition based attendance system.
1. Clone the project
	git clone the project to your machine.
2. Installing virtual environment
Install a virtual environment so that all the dependant libraries can be installed separately.
	i. Creating a virtual environment
		pip install virtualenv
		virtualenv {name of the virtual environment}
To use the virtual environment, activate the virtual environment created in the step above.
	ii. Activating the virtual environment
{name of the virtual environment}\Scripts\activate
3. Installing the requirements
	pip install -r requirements.txt
4. Recording training images
Inorder to verify if the detected face is of a particular person or not, we first have to train our algorithm with images of the students in the class. This can be done by first storing the images in “Training_images” folder. Please make sure you provide the same name to the folder in which you save all the training images.
Save the images with the name of the person (jpg or png).
5. Training and Testing the algorithm 
open the command prompt and run the python file named “facerecognition.py” by inserting the command “python facerecognition.py”
Once the algorithm is run, the dlib library and the opencv library trains the algorithm with the faces stored in the “training_images” folder and generates encodings for each face. Once the training is done, you should be able to see your webcam opened and capture the video and place a bounding box on all the faces detected. If there is a name stored for that particular detected face, algorithm should display the name on the bounding box.
