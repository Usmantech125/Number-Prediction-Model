# Step-by-Step Explanation

Step 1: Import tools we need
We use libraries (like tools in a toolbox):

tensorflow.keras: helps us build and train a neural network.

numpy: helps with numbers and arrays.

matplotlib.pyplot: helps us show images.

random: to pick random images.

Step 2: Load the MNIST dataset
MNIST is a free set of 28x28 grayscale images of digits 0–9.

X_train: images for training (learning)

y_train: the correct answers for those images

X_test: new images we’ll test the model on

y_test: the correct answers for test images

Step 3: Preprocess the data
We reshape the data to say: “Each image is 28x28 pixels, and it has 1 color channel (black & white).”
We divide by 255.0 so all pixel values are between 0 and 1 — easier for the model to learn.
Then we turn the labels into a "one-hot" format.

Step 4: Build the model (the brain)
We create a Convolutional Neural Network (CNN) that finds patterns like lines and curves in the image, flattens it, and makes a guess.

Step 5: Compile the model
We tell the model how to learn (using Adam), what to minimize (loss), and what to measure (accuracy).

Step 6: Train the model
The model looks at images and the correct answers, learns the patterns, and adjusts itself over 5 rounds (epochs).

Step 7: Test the model
We give it new images it hasn’t seen before and check how many it gets right.

Step 8: Predict a new digit
We show the model a random image from the test set and it predicts what digit it sees.
