# CNN_Model_Melanoma
assignment on detection of Melanoma using CNN based model

1. Data Reading & Understanding
Data Source: The dataset consists of 2357 images categorized into 9 different skin conditions:
Actinic keratosis
Basal cell carcinoma
Dermatofibroma
Melanoma
Nevus
Pigmented benign keratosis
Seborrheic keratosis
Squamous cell carcinoma
Vascular lesion
Key Task:
Read the data, define paths for the training and testing images, and inspect the image metadata.
Ensure proper file structure to load the images correctly in the TensorFlow pipeline.

2. Dataset Creation
Train-Validation Split:
Divide the dataset into training and validation datasets.
Use a batch size of 32 and resize the images to a uniform size of 180x180.
Utilize TensorFlow’s ImageDataGenerator for loading images and performing data augmentation if needed later.

3. Dataset Visualization
Visualize one image instance from each of the 9 classes to understand the data better.
Plot a grid of 3x3 images, each representing one of the disease classes.

4. Initial Model Building & Training
CNN Architecture:
Build a custom CNN model with layers such as Conv2D, MaxPooling2D, Dense, Dropout, and Flatten. Normalize pixel values between (0, 1).
Example structure:
Input: 180x180x3
Conv2D → MaxPooling2D → Conv2D → MaxPooling2D → Flatten → Dense (output layer with 9 units for multiclass classification)


Training: Train the model for 20 epochs using categorical cross-entropy as the loss function and an appropriate optimizer like Adam.
Findings: After training, assess if there's overfitting or underfitting by comparing the training and validation accuracy/loss.
5. Data Augmentation to Resolve Underfitting/Overfitting
If the model is overfitting (i.e., the training accuracy is high, but validation accuracy is low), introduce data augmentation to increase image diversity and improve generalization.
Data Augmentation Techniques: Apply transformations such as rotation, zoom, flip, and shear.

6. Model Building & Training on Augmented Data
Retrain the CNN model with the augmented data.
Compare the performance of this model with the earlier one to see if overfitting/underfitting issues are resolved.
7. Class Distribution Examination
Examine class imbalance by checking the number of samples in each class.
Question:
Which class has the least samples?
Which class dominates in terms of sample size?

8. Handling Class Imbalance
If class imbalance exists, apply resampling techniques (like oversampling minority classes or undersampling dominant classes).
Use the Augmentor library to balance the dataset.
9. Model Training on Rectified Data
Re-train the model on the balanced dataset for 30 epochs.
Evaluate the performance of the new model and observe if class imbalance issues are resolved.

