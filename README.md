
# 🎬 Movie Review Sentiment Classification (IMDB Dataset)

A deep learning project for **sentiment analysis** on the IMDB dataset, classifying movie reviews as **positive** or **negative** using a simple neural network built with Keras. The project covers preprocessing, one-hot encoding, model training, validation, and visualization of results.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📖 Overview
This project demonstrates a **binary classification** task using the **IMDB Movie Reviews Dataset**.  
The goal is to classify reviews as **positive** or **negative** based on their textual content.  

The project uses **Keras** and a simple **fully connected neural network** to build and train the sentiment analysis model.  
It highlights the end-to-end workflow: text preprocessing → vectorization → model building → training → evaluation.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🎯 Objectives
- Classify IMDB movie reviews into **positive (1)** or **negative (0)**.  
- Understand the workflow of text preprocessing, feature extraction, and training a neural network.  
- Explore **overfitting** and the role of validation data.  
- Visualize the training process using **loss and accuracy plots**.  

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## ⚙️ Features
- Preprocessing and vectorization of raw text reviews.  
- **Neural Network** built using Keras:  
  - Two hidden `Dense(16, activation='relu')` layers.  
  - One output `Dense(1, activation='sigmoid')` layer.  
- Optimizer: **RMSprop** (lr=0.001).  
- Loss function: **Binary Crossentropy**.  
- Validation set of 10,000 samples for monitoring generalization.  
- Training and validation curves for **loss** and **accuracy**.  

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🛠 Tools & Technologies  
- **Python 3.x**  
- **TensorFlow / Keras** – Model building and training  
- **NumPy** – Numerical operations  
- **Matplotlib** – Visualization  
- **Jupyter Notebook / VS Code** – Development environment


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📊 Dataset  
- **Name**: IMDB Movie Review Dataset  
- **Size**: 50,000 reviews  
  - 25,000 reviews for **training** (50% positive, 50% negative)  
  - 25,000 reviews for **testing** (50% positive, 50% negative)  
- **Source**: [IMDB Dataset (Keras)](https://keras.io/api/datasets/imdb/)  
- **Preprocessing**:  
  - Reviews converted into sequences of integers (word indices).  
  - Restricted to the **top 10,000 most frequent words**.  
  - Labels: `0 = Negative`, `1 = Positive`.  

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 🏗️ Model Architecture  
- **Input Layer**: 10,000-dimensional one-hot encoded vectors.  
- **Hidden Layers**:  
  - `Dense(16, activation='relu')`  
  - `Dense(16, activation='relu')`  
- **Output Layer**:  
  - `Dense(1, activation='sigmoid')` → probability (0 to 1).  
- **Optimizer**: RMSprop (lr=0.001)  
- **Loss Function**: Binary Crossentropy  
- **Metrics**: Accuracy  

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📈 Results  

### Training vs Validation  
- Training accuracy improves with epochs.  
- Validation accuracy peaks around **epoch 4–5** before **overfitting** begins.

- Training vs Validation Loss:

<img width="567" height="455" alt="image" src="https://github.com/user-attachments/assets/af38db6c-4eba-412b-9837-80148a8afafe" />


- Training vs Validation Accuracy:

  <img width="584" height="455" alt="image" src="https://github.com/user-attachments/assets/d34d33e7-b1ae-4372-a853-ccf88eea4300" />


### Model Performance on Test Data  
- **Confusion Matrix** ✅ (visualized with Seaborn).  
- **Classification Report** ✅ (precision, recall, F1-score).  

Example performance (values may vary slightly due to random initialization):  

| Metric    | Negative | Positive |
|-----------|----------|----------|
| Precision | 0.89     | 0.87     |
| Recall    | 0.86     | 0.89     |
| F1-score  | 0.88     | 0.88     |

- **Overall Accuracy**: ~88%

- Confusion Matrix:

<img width="531" height="470" alt="image" src="https://github.com/user-attachments/assets/8706d1f3-e515-4c6c-94a7-e302bd99a0e6" />


### Example Prediction  
```text
Review: "This movie was amazing! The acting was great and the story was touching."
Predicted Sentiment: Positive
```

<img width="846" height="313" alt="movie-review" src="https://github.com/user-attachments/assets/b54b3bc5-b2af-4d74-a78d-0b202e39c283" />


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📌 References  

1. [IMDB Large Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)  
2. [IMDB Dataset Paper – Maas et al., 2011](https://ai.stanford.edu/~amaas/papers/wvSent_acl2011.pdf)   
3. [Keras IMDB Dataset Documentation](https://keras.io/api/datasets/imdb/)  

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 👤 Author

Muqadas Ejaz

BS Computer Science (AI Specialization)

AI/ML Engineer

Data Science & Gen AI Enthusiast

📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/muqadasejaz/)  

🌐 GitHub: [github.com/muqadasejaz](https://github.com/muqadasejaz)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## 📎 License

This project is open-source and available under the [MIT License](LICENSE).

