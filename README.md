Build a simple fully connected neural-network (Multi-Layer Perceptron) to classify images in the [Fashion MNIST](https://www.kaggle.com/datasets/zalando-research/fashionmnist) dataset and visualize the results with a confusion matrix and per-class accuracy bar chart.

---

## 📌 Project Question
> *Build an image classifier using the Fashion MNIST dataset to categorize clothing items. Visualize results using a confusion matrix.*

---

## 🗂 Dataset

| Property | Value |
|----------|-------|
| *Name* | Fashion MNIST |
| *Size* | 70 000 28 × 28 grayscale images |
| *Split* | 60 000 train / 10 000 test |
| *Classes* | T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot |

Keras can download the dataset automatically, so no manual download is required.

---

## 🏗 Methodology

1. *Load & Normalize*  
   Scale pixel values to [0, 1] for faster convergence.
2. *One-hot Encode Labels*  
   Convert integer class IDs to categorical vectors.
3. *Model Architecture*  
   * Flatten → Dense(128, ReLU) → Dense(64, ReLU) → Dense(10, softmax)
4. *Compile*  
   * Optimizer  : *Adam*  
   * Loss       : *Categorical Cross-Entropy*  
   * Metric     : *Accuracy*
5. *Train* for *5 epochs* with a *10 % validation split*.
6. *Evaluate* on the test set.
7. *Visualize*  
   * Confusion matrix (Seaborn heat-map)  
   * Per-class recall bar chart

---

## 🔧 Requirements

| Package | Version (or higher) |
|---------|---------------------|
| Python  | 3.8+ |
| TensorFlow | 2.x |
| NumPy | 1.x |
| Matplotlib | 3.x |
| Seaborn | 0.12+ |
| Pandas | 1.x |
| scikit-learn | 1.x |

Install everything in one go:

bash
pip install tensorflow matplotlib seaborn pandas scikit-learn


---

## 🚀 Quick Start

Clone the repo and run the script (works in VS Code, terminal, or Google Colab):

bash
git clone https://github.com/<your-username>/fashion-item-classification.git
cd fashion-item-classification
python fashion_mnist_dense.py


---

## 🖼 Example Output

| Metric | Value (typical) |
|--------|-----------------|
| *Overall Test Accuracy* | ~0.88 |

> Add screenshots of confusion matrix and per-class accuracy here.

---

## 📜 Full Code

See fashion_mnist_dense.py in this repo for the complete commented code.

---

## 🧑‍💻 Author

| Field | Information |
|-------|-------------|
| *Name* | Divyansh Verma |
| *Roll No. / ID* | 202401100400084 |
| *Institute* | KIET Group of Institutions |

---

## 📄 License

This repository is released for educational purposes under the MIT License.  
Feel free to use or adapt the code—please credit the original author.
