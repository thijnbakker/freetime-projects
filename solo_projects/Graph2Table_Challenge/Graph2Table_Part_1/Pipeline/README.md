# Image Classification Project

This repository contains three main Jupyter notebooks that together handle dataset cleaning, model training, and model inference for an image classification task.

## Project Structure

- **A_clean_dataset.ipynb**: 
  - Preprocess and clean the image dataset.
  - Organize images into train/validation/test folders.
  - Resize or reformat images if necessary.

- **B_C_D_train_model_v4.ipynb**:
  - Define a Convolutional Neural Network (CNN) architecture using TensorFlow/Keras.
  - Train the model with data augmentation.
  - Apply callbacks like EarlyStopping and ReduceLROnPlateau to improve training.
  - Evaluate the model performance.

- **E_model_inference.ipynb**:
  - Load a trained model.
  - Perform inference on new/unseen images.
  - Visualize predictions.

## Requirements

See [requirements.txt](requirements.txt) for a full list of required Python libraries.

## How to Run

1. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the notebooks in order:
    - First, clean and prepare the dataset (`A_clean_dataset.ipynb`).
    - Then, train the model (`B_C_D_train_model_v4.ipynb`).
    - Finally, run inference using the trained model (`E_model_inference.ipynb`).

## Notes

- This project uses TensorFlow/Keras for model training and inference.
- Make sure you have a GPU-enabled environment for faster training (optional but recommended).
- Dataset structure should match the expected format after preprocessing (organized by class folders).

---
