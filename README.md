#  Food-101 Classifier Web App

An interactive computer vision web application built with **PyTorch** and **Streamlit** that classifies dishes across **101 distinct food categories** using deep transfer learning.


[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://food-101-classifier-app.streamlit.app/)
[![GitHub stars](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

---

## 📌 Features

- **Multi-Class Food Classification:** Recognizes 101 diverse culinary dishes from the Food-101 benchmark dataset.
- **Top Predictions & Probabilities:** Returns ranked class probabilities and confidence scores for uploaded food photos.
- **Fast Inference:** Lightweight image transformation pipeline running on PyTorch CPU.
- **Clean Interactive UI:** Built using Streamlit for instant image upload and live evaluation in a sleek dark theme.

---

## 🛠️ Tech Stack

- **Deep Learning Framework:** PyTorch, Torchvision
- **Frontend / Deployment:** Streamlit
- **Image Processing:** Pillow (PIL), NumPy
- **Base Architecture:** EfficientNet-B3 (Pretrained on ImageNet with a custom classification head)

---

##  Getting Started

### 1. Clone the Repository
```bash
git clone [https://github.com/vikassinngh123/food-101-classifier-app.git](https://github.com/vikassinngh123/food-101-classifier-app.git)
cd food-101-classifier-app
```

### 2. Set Up a Virtual Environment (Recommended)
```bash
python -m venv venv

# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit Application
```bash
streamlit run food101_app.py
```
*The app will automatically open in your browser at `http://localhost:8501`.*

---

## 📂 Project Organization

- `food101_app.py`: The Streamlit frontend UI and application logic.
- `food101_utils.py`: PyTorch inference helpers, including model caching and image transformations.
- `food101_model.py`: EfficientNet-B3 architecture definition and custom head setup.
- `food101_dataset.py`: PyTorch `DataLoader` and torchvision transformation logic.
- `model_training_and_evaluation.ipynb`: The core data science notebook containing EDA, training loops, metrics, and visualization.
- `food101_classes.json`: Dictionary mapping for the 101 dataset classes.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.