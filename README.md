#  Grape Leaf Disease Detection and Pesticide Recommendation

##  Project Overview

This project is a deep learning-based application designed to detect diseases in grape leaves from uploaded images. The system uses a **Convolutional Neural Network (CNN)** to classify grape leaf images and provides appropriate pesticide recommendations based on the predicted disease.

The project also includes an interactive **Streamlit web application** where users can upload an image of a grape leaf and receive the prediction result along with the confidence score and treatment recommendation.

---

##  Objectives

* Detect grape leaf diseases using deep learning.
* Classify grape leaves into different disease categories.
* Compare the performance of CNN and ANN models.
* Provide pesticide recommendations based on the detected disease.
* Build a user-friendly web interface using Streamlit.

---

##  Disease Classes

The model can classify grape leaves into the following four categories:

1. **Black Rot**
2. **Esca (Black Measles)**
3. **Healthy**
4. **Leaf Blight (Isariopsis Leaf Spot)**

---

##  Technologies Used

* Python
* PyTorch
* TensorFlow / Keras
* Streamlit
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* PIL (Python Imaging Library)

---

## Model Development

The project uses a **Convolutional Neural Network (CNN)** for image classification.

### Image Preprocessing

The input images are:

* Resized to **224 × 224 pixels**
* Converted into tensors
* Normalized before training
* Loaded using PyTorch DataLoaders

### CNN Architecture

The CNN model includes:

* Convolutional layers
* ReLU activation
* Max Pooling layers
* Fully Connected layers
* Softmax-based classification

The model was trained to identify different grape leaf diseases from image data.

---

##  Model Evaluation

The model was evaluated using:

* Accuracy
* Loss
* Classification Report
* Precision
* Recall
* F1-Score

The project also compares the performance of:

* **CNN Model**
* **ANN Model**

The results showed that the CNN model performed better for image classification.

---

##  Web Application

The project includes a Streamlit application where users can:

1. Upload a grape leaf image.
2. Allow the model to analyze the image.
3. View the predicted disease.
4. View the prediction confidence.
5. Receive a pesticide recommendation.

---

##  Pesticide Recommendations

| Disease              | Recommendation                                                           |
| -------------------- | ------------------------------------------------------------------------ |
| Black Rot            | Use fungicides such as myclobutanil or mancozeb                          |
| Esca (Black Measles) | Use fungicides like tebuconazole or carbendazim and prune affected areas |
| Healthy              | No pesticide needed. Continue monitoring the plant                       |
| Leaf Blight          | Use fungicides such as chlorothalonil or copper-based sprays             |

---

##  Application Workflow

```text
Upload Grape Leaf Image
          ↓
Image Preprocessing
          ↓
CNN Model Prediction
          ↓
Disease Classification
          ↓
Confidence Score
          ↓
Pesticide Recommendation
```

---

##  Project Structure

```text
Grape-Leaf-Disease-Detection/
│
├── grape_leaf_disease_detection_and_pestiside_recommendation.ipynb
│   └── Model training and evaluation
│
├── main.py
│   └── Streamlit application
│
├── trained_model.pkl
│   └── Trained model
│
├── grape_leaf_model.h5
│   └── Model used for prediction
│
├── dataset/
│   ├── train/
│   └── test/
│
└── README.md
```

---

##  Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/grape-leaf-disease-detection.git
```

### 2. Navigate to the project folder

```bash
cd grape-leaf-disease-detection
```

### 3. Install required libraries

```bash
pip install streamlit tensorflow torch torchvision numpy pandas matplotlib seaborn scikit-learn pillow
```

---

##  Run the Application

Run the following command:

```bash
streamlit run main.py
```

After running the command, the application will open in your browser.

---

## Application Screenshots

Add screenshots of your application here.

```text
![Home Page](images/home.png)

![Prediction Result](images/result.png)
```

---

##  Future Improvements

* Improve model accuracy using transfer learning.
* Add more grape leaf disease classes.
* Deploy the application online.
* Support real-time camera-based disease detection.
* Add disease prevention and treatment information.
* Improve the user interface.

---



---

## 📄 Conclusion

This project demonstrates the application of deep learning and computer vision in agriculture. By analyzing grape leaf images, the system helps identify diseases and provides pesticide recommendations, which can support farmers in taking early action to protect their crops.
