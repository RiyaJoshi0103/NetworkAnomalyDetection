# Network Anomaly Detection using PCA and Clustering

## 📌 Objective
To detect anomalies in network traffic data using dimensionality reduction (PCA), clustering (DBSCAN), and classification (LOF, KNN, Random Forest) techniques.

---

## 📁 Dataset
- File used: `all_data.csv`
- Columns include categorical and numerical features with a target column named `class`.

---

## 🛠️ Tools & Technologies
- **Language**: Python
- **Libraries**: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn
- **Models Used**:
  - DBSCAN (for clustering)
  - Local Outlier Factor (LOF)
  - K-Nearest Neighbors (KNN)
  - Random Forest Classifier

---

## 🔍 Process Overview

### 1. **Data Preprocessing**
- Loaded CSV file.
- Checked for nulls and class distribution.
- Visualized feature distributions using `hist()`.

### 2. **Encoding and Scaling**
- Encoded target class using `OrdinalEncoder`.
- Scaled entire dataset using `StandardScaler`.

### 3. **Dimensionality Reduction**
- Applied PCA to retain 95% of the variance.
- Reduced dimensions used for clustering and visualization.

### 4. **Clustering (DBSCAN)**
- Applied DBSCAN to detect outliers/anomalies.
- Cluster labels were added as a new column `type`.
- Label `-1` was converted to "anomalous", others to "normal".

### 5. **Data Visualization**
- Countplot of normal vs. anomalous points.
- Scatter plot of PCA components color-coded by anomaly type.

### 6. **Model Building**
#### a. Local Outlier Factor (LOF)
- Used `novelty=True` and `contamination=0.013`
- Accuracy computed on test data.

#### b. Random Forest (Tested on Iris dataset as demonstration)
- Trained and evaluated using classification report and confusion matrix.

#### c. K-Nearest Neighbors
- Trained on split data.
- Accuracy, confusion matrix, and classification report printed.

#### d. Cross-Validation
- Performed 5-fold cross-validation on KNN.
- Reported average accuracy.

---

## 📊 Evaluation Metrics
- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report**
- **F1 Score**
- **Normalized Confusion Matrix**

---

## 📌 Improvements to be Made
- Train Random Forest on actual anomaly detection dataset instead of the Iris dataset.
- Save plots using `plt.savefig()` to include in the GitHub repository.
- Improve class balance via oversampling or SMOTE.
- Implement real-time data stream detection (Kafka, PySpark).

---

## 📷 Screenshots
You can add screenshots of:
- Confusion matrix
- Countplots
- PCA scatterplots

(Add them in a `/plots` folder and reference like `![Confusion Matrix](plots/confusion_matrix.png)`)

---

## 👤 Author
- **Your Name**
- [LinkedIn Profile] | [GitHub Profile] | [Portfolio Link]

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
