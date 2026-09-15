# 👕 Deep Learning Fashion Image Classification

A simple **Deep Learning image classification project** built with **Python, TensorFlow/Keras, and Fashion MNIST**. The project demonstrates how an Artificial Neural Network can learn from fashion product images and predict their product categories.

## 📌 Project Overview

In an e-commerce business, thousands of product images may need to be categorized before products are added to an online store. Manually categorizing every image can be repetitive and time-consuming.

This project demonstrates an AI-assisted approach where a Deep Learning model analyzes a product image and predicts its category.

**Input:** Fashion product image
**Output:** Predicted product category

The project is designed as a practical demonstration for **BBA AI/ML students**.

## 🎯 Objectives

* Understand how images can be used as input for Deep Learning.
* Build a simple Artificial Neural Network.
* Understand input, hidden, and output layers.
* Train a model on fashion product images.
* Evaluate model accuracy.
* Predict the category of an unseen image.
* Understand the business applications of image classification.

## 📊 Dataset

The project uses the **Fashion MNIST** dataset, which contains grayscale images of fashion products.

The model classifies images into 10 categories:

1. T-shirt/Top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle Boot

The dataset is loaded directly through TensorFlow/Keras, so no manual dataset upload is required.

## 🧠 Model Architecture

The project uses a simple Artificial Neural Network:

```text
Input Image (28 × 28)
        ↓
Flatten Layer
        ↓
Dense Layer (64 neurons)
        ↓
ReLU Activation
        ↓
Output Layer (10 neurons)
        ↓
Softmax
        ↓
Predicted Fashion Category
```

The `Flatten` layer prepares the image data, the `Dense(64)` layer acts as the hidden layer, and the final 10-neuron layer represents the 10 product categories. Softmax produces category probabilities.

## ⚙️ Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **NumPy**
* **Matplotlib**
* **Fashion MNIST**

## 🔄 Project Workflow

```text
Fashion MNIST Dataset
        ↓
Load Images
        ↓
Visualize Images
        ↓
Normalize Pixel Values
        ↓
Build Neural Network
        ↓
Compile Model
        ↓
Train Model
        ↓
Evaluate Accuracy
        ↓
Make Predictions
        ↓
Compare Predicted vs Actual Category
```

The image pixel values are normalized from **0–255 to 0–1** before training. The model is trained for **3 epochs** with a 10% validation split.

## 📈 Model Evaluation

The model is evaluated on test images that were not used during training.

The notebook calculates and displays the test accuracy:

```python
test_loss, test_accuracy = model.evaluate(
    test_images,
    test_labels,
    verbose=0
)

print("Test Accuracy:", round(test_accuracy * 100, 2), "%")
```

The exact accuracy can vary slightly when the notebook is executed.

## 🔮 Prediction

After training, the model predicts the category of an image and compares it with the actual category.

Example:

```text
Predicted Product: Sneaker
Actual Product: Sneaker
```

The notebook also allows different test images to be selected and classified.

## 💼 Business Application

A major application of this project is **fashion e-commerce**.

### Traditional Process

```text
Product Image
     ↓
Employee manually selects category
     ↓
Product added to website
```

### AI-Assisted Process

```text
Product Image
     ↓
Deep Learning Model
     ↓
Predicted Category
     ↓
Employee Review (if required)
     ↓
Product added to website
```

### Possible Business Benefits

* ⚡ Faster product listing
* 👨‍💻 Reduced repetitive manual work
* 📂 More consistent product categorization
* 🔎 Better product-search experience
* 📈 Ability to process a larger number of images

## ⚠️ Limitations

The model's predictions are not always correct. Therefore, accuracy alone should not be the only factor considered before deploying an AI system.

Businesses should also consider:

* Cost of incorrect classification
* Customer experience
* Quality of training data
* Human review
* Overall business risk

## 📁 Repository Structure

```text
deep-learning-fashion-image-classification/
│
├── Deep_Learning_Fashion_Image_Classification_BBA.ipynb
├── README.md
│
└── part-a/
    └── deep-learning/
        └── Deep_Learning_Fashion_Classification_Name.ipynb
```

The course submission instructions suggest placing the project under:

```text
part-a/deep-learning/
```

and uploading the notebook along with a screenshot showing the product image, predicted category, and actual category.

## 📝 Key Takeaways

* Deep Learning can learn patterns from images.
* Artificial Neural Networks contain input, hidden, and output stages.
* Training allows a model to learn from historical examples.
* Testing evaluates performance on unseen examples.
* A trained model can predict the category of a new image.
* AI predictions can be incorrect.
* Human oversight can remain important in business AI applications.

## 👨‍🎓 Academic Project

**Project:** Deep Learning Fashion Image Classification
**Area:** Artificial Intelligence / Machine Learning
**Application:** E-commerce Product Classification
**Framework:** TensorFlow/Keras
**Dataset:** Fashion MNIST
**Model:** Artificial Neural Network

---

⭐ *This project demonstrates how Deep Learning can be connected with a practical business problem in e-commerce.*
# deep-learning-fashion-image-classification
Deep Learning project using TensorFlow/Keras to classify fashion product images into 10 categories using the Fashion MNIST dataset, with an e-commerce business use case.
