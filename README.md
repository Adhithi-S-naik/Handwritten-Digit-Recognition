# Handwritten Digit Recognition

This project uses a neural network built with **TensorFlow/Keras** to recognize handwritten digits (0–9) from image data. It’s developed and trained in **Google Colab**.

---

## Dataset Information

- The dataset (`Train.csv`) contains **42,000** labeled images of handwritten digits.
- Each image is **28x28 pixels**, flattened into 784 pixel values.
- The dataset is **not stored in this GitHub repository** due to size limits.
- It is stored in **Google Drive**, and the Colab notebook uses `gdown` to download it at runtime.

---

## How to Run

1. Open the Colab notebook:  
   [`Handwritten_Digit_Recognition.ipynb`](./Handwritten_Digit_Recognition.ipynb)

2. Run the first cell to download the dataset from Google Drive:
   ```python
   import gdown

   file_id = '1kaOpVsT4QX6PK0zhFx86gN6Yhoy6DF6K' 
   url = f'https://drive.google.com/uc?id={file_id}'
   gdown.download(url, 'Train.csv', quiet=False)
   
3. Proceed to train the model and visualize predictions.

# Technologies Used
      1. Python 3.x
      2. NumPy, pandas, matplotlib
      3. TensorFlow / Keras
      4. scikit-learn
      5. Google Colab
      6. gdown (for downloading the dataset)

# Results
      1. Training Accuracy: ~96.8%
      2. Validation Accuracy: ~97.1%
      3. Visualization of predictions for sample test images
