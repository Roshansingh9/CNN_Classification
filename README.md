# CNN Image Classification — Learning Project

This project is a Jupyter Notebook where I practice building and training a Convolutional Neural Network (CNN) for image classification using TensorFlow and Keras. The code demonstrates the full workflow: loading images, preprocessing, defining a CNN, training, and evaluating the model.

---

## 📚 What This Project Covers

- **Loading image data** from folders using `image_dataset_from_directory`
- **Normalizing images** to the [0, 1] range for better training stability
- **Building a CNN** with multiple convolutional and pooling layers
- **Compiling and training** the model for binary classification
- **Evaluating** model performance on a validation set

---

## 🗂️ Project Structure

```
CNN_Classification/
│
├── CNN.ipynb         # Main notebook with all code and explanations
├── train/            # Folder with training images (subfolders per class)
└── test/             # Folder with validation images (subfolders per class)
```

---

## 🚀 How to Run

1. **Prepare your data:**  
   Place your images in the `train` and `test` folders, each with subfolders for each class (e.g., `train/cats`, `train/dogs`).

2. **Install dependencies:**  
   Make sure you have Python 3.7+ and install the required packages:
   ```sh
   pip install tensorflow keras
   ```

3. **Open the notebook:**  
   Open `CNN.ipynb` in Jupyter Notebook or VS Code.

4. **Run the cells:**  
   Step through each cell to:
   - Load and preprocess the data
   - Build and summarize the CNN model
   - Compile and train the model
   - View training results

---

## 🏗️ Model Architecture

- **Input:** 256x256 RGB images
- **Layers:**
  - 3 × [Conv2D + MaxPooling2D]
  - Flatten
  - Dense(128, relu)
  - Dense(64, relu)
  - Dense(1, sigmoid) — for binary classification

---

## 💡 What I Learned

- How to use Keras utilities to load and preprocess image datasets
- How to design a basic CNN for image classification
- The importance of normalization and model evaluation

---

## 📎 References

- [TensorFlow Image Classification Guide](https://www.tensorflow.org/tutorials/images/classification)
- [Keras Documentation](https://keras.io/api/)

---

*This notebook is for learning and experimentation purposes only.*