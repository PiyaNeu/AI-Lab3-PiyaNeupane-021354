# Machine Learning with k-Nearest Neighbors (kNN)

This repository contains a custom-built implementation of the **k-Nearest Neighbors** algorithm in Python. The focus is on understanding how kNN works internally without relying on external ML libraries like scikit-learn.

You’ll find examples for:
- Binary classification based on two features (e.g., height and weight)
- Multi-class classification using flower measurements
- Visualization of how the decision boundaries change with data

---

## Project Files

| File | Purpose |
|------|---------|
| `knn_binary_classification.py` | Performs binary classification using manually coded kNN |
| `knn_multiclass_classification.py` | Implements kNN for predicting among three categories |
| `knn_visualization.py` | Visualizes decision boundaries for a 2D binary classification case |
| `README.md` | Documentation for using and understanding the code |

---

### 1️⃣ Binary Classification (2D Feature Space)

- **Input Features**: Height and Weight
- **Target Labels**: `1 = Pass`, `0 = Fail`
- **k-value**: `k = 3`
- **Details**:
  - Computes distance between new and training data using **Euclidean Distance**
  - Classifies based on the most frequent label among the 3 nearest neighbors

---

### 2️⃣ Multi-Class Classification (3D Feature Space)

- **Input Features**: Sepal Length, Sepal Width, Petal Length
- **Classes**:  
  - `0 = Species A`  
  - `1 = Species B`  
  - `2 = Species C`
- **k-value**: `k = 5`
- Uses a similar logic to binary classification, but picks the most common class among top 5 neighbors

---

### 3️⃣ 📊 Decision Boundary Visualization

- Visualizes how the kNN algorithm splits the feature space
- Uses a **mesh grid** to evaluate predictions across a region
- Shows scatter plot with colored regions representing predicted classes

---

## ▶️ How to Run

### 🔧 Requirements
- Python 3.x
- `matplotlib` and `numpy` installed

### 💻 Execute the Scripts
Run in terminal or command prompt:

```bash
python knn_binary_classification.py
python knn_multiclass_classification.py
python knn_visualization.py
