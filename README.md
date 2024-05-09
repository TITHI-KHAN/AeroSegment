# AeroSegment

## Dataset

Semantic segmentation dataset : https://www.kaggle.com/datasets/mejbahahammad/semantic-segmentation-dataset/

Semantic segmentation of aerial imagery : https://www.kaggle.com/datasets/humansintheloop/semantic-segmentation-of-aerial-imagery

### Step-by-Step Explanation:

1. **Import Libraries:**
   - Libraries like `os`, `numpy`, `tensorflow`, and related modules are imported. These are common libraries for data manipulation, numerical operations, and deep learning.

2. **Define Paths and Load Data:**
   - Set the path to the dataset directory.
   - Load image and mask file paths into lists.

3. **Define Image and Mask Processing Function:**
   - Function `process_images_masks` processes images and masks from directories. It reads images and masks, resizes them, and collects them into numpy arrays.

4. **Define Data Augmentation Generator Function:**
   - Function `create_augmentation_datagen` creates an image data generator for data augmentation purposes using Keras' `ImageDataGenerator`.

5. **Generate Augmented Data:**
   - Augment data using the defined data augmentation generator.

6. **Define UNet Model Architecture:**
   - Define functions for creating the convolutional blocks and the UNet model itself.

7. **Create UNet Model Instance:**
   - Create an instance of the UNet model using the defined architecture.

8. **Define Training Generator Function:**
   - Define a function `train_generator_func` that yields batches of images and masks indefinitely.

9. **Create Final Training Generator:**
   - Create the final training generator using the defined function and the augmented image and mask generators.

10. **Train the Model:**
    - Train the UNet model using the final training generator. Adjust parameters like steps per epoch and number of epochs as needed.

11. **Save Trained Model:**
    - Save the trained model to a file.

12. **Optional: Plot Training History:**
    - Plot training history (loss and accuracy) for analysis.


