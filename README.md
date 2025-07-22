CNN CIFAR-10 Image Classifier

This repository contains a complete implementation of a **Convolutional Neural Network (CNN)** built from scratch using **TensorFlow** and **Keras** for classifying images from the **CIFAR-10** dataset.

---

## 📌 Project Overview

- **Objective**: Build and train a CNN to classify 60,000 32x32 color images into 10 categories (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck).
- **Model**: Custom-designed CNN architecture using Conv2D, MaxPooling2D, Dropout, and Dense layers.
- **Training**: Conducted over **5 epochs** with performance tracking.
- **Evaluation**: Includes accuracy and loss metrics for training and validation sets with visualization using Matplotlib.

---

## 📁 Dataset: CIFAR-10

- **Training Images**: 50,000
- **Test Images**: 10,000
- **Classes**:  
  `['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']`
- **Input Size**: 32x32 RGB (3 channels)

---

## 🏗️ Model Architecture

```text
Input (32x32x3)
│
├── Conv2D (32 filters, 3x3) + ReLU
├── MaxPooling2D (2x2)
│
├── Conv2D (64 filters, 3x3) + ReLU
├── MaxPooling2D (2x2)
│
├── Conv2D (128 filters, 3x3) + ReLU
├── MaxPooling2D (2x2)
│
├── Flatten
├── Dense (128) + ReLU
├── Dropout (0.3)
└── Dense (10) + Softmax
````

---

## ⚙️ Tools & Technologies

* Programming Language: **Python 3.x**
* Frameworks: **TensorFlow 2.x**, **Keras**
* Visualization: **Matplotlib**
* Data Handling: **NumPy**

---

## 📊 Training Configuration

| Parameter     | Value                           |
| ------------- | ------------------------------- |
| Epochs        | 5                               |
| Batch Size    | 32 (default)                    |
| Optimizer     | Adam                            |
| Loss Function | Categorical Crossentropy        |
| Metrics       | Accuracy                        |
| Activation    | ReLU (hidden), Softmax (output) |

---

## 📈 Results & Visualization

* Trained model for 5 epochs.
* Plotted training and validation accuracy & loss to track performance.

<p align="center">
  <img src="results/accuracy_plot.png" width="400"/>
  <img src="results/loss_plot.png" width="400"/>
</p>

> *(Include the plots in a folder named `/results` if you'd like them visible in README.)*

---

## ▶️ Getting Started

### 🔧 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/cnn-cifar10-image-classifier.git
   cd cnn-cifar10-image-classifier
   ```

2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open and run: `Epochs - 5.ipynb`

---

## 🧾 Requirements

Create a `requirements.txt` file with the following:

```txt
tensorflow
numpy
matplotlib
```

> You can generate it using:
>
> ```bash
> pip freeze > requirements.txt
> ```

---

## 📝 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

Feel free to fork this repository, raise issues, or submit pull requests for improvements.

---

## 📫 Contact

For project-related inquiries or collaboration requests:
📧 [basakupangshu70@gmail.com](mailto:basakupangshu70@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/upangshu-basak/)
