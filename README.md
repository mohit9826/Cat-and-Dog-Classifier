Model Training:
python3 train.py

Using TensorBoard:
tensorboard --logdir=Data/Checkpoints/./logs

Model Architecture:
Input Data Shape: 64x64x3
Layer 1:

Convolutional Layer 32 filter Filter shape: 3x3

Activation Function: ReLu

Max Pooling Pool shape: 2x2

Layer 2:

Convolutional Layer 32 filter Filter shape: 3x3

Activation Function: ReLu

Max Pooling Pool shape: 2x2

Layer 3:

Convolutional Layer 64 filter Filter shape: 3x3

Activation Function: ReLu

Max Pooling Pool shape: 2x2

Classification:

Flatten

Dense Size: 64

Activation Function: ReLu

Dropout Rate: 0.5

Dense Size: 2

Activation Function: Sigmoid

Optimizer: Adadelta
Loss: Binary Crossentropy
Adding new train dataset:
If you want to add new dataset to datasets, you create a directory and rename what you want to add category (like 'cat' or 'phone').

If you want to add a new training image to previously category datasets, you add a image to about category directory and if you have npy files in Data folder delete npy_train_data folder.

Note: We work on 64x64 image also if you use bigger or smaller, program will automatically return to 64x64.

Important Notes:
Used Python Version: 3.6.0
Install necessary modules with sudo pip3 install -r requirements.txt command.
