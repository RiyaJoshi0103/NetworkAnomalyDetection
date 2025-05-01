
# Network Anomaly Detection using Machine Learning

## 📌 Objective
To analyze network traffic data and detect anomalies that may indicate malicious activity or system errors using data visualization and machine learning models.

## 📈 Dataset Overview
- A CSV file (`network_traffic.csv`) contains time-based network traffic records.
- Columns include: `Timestamp`, `Packets`, `Bytes`, `Source`, `Destination`, and `Label` (Normal/Anomalous).

## ⚙️ Technologies Used
- **Python**
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Tools**: Jupyter Notebook, VS Code

## 🔬 Exploratory Data Analysis (EDA)
Using **Seaborn** and **Matplotlib**, the following visualizations were generated:
- **Lineplot of Packets over Time**: to understand traffic trends.
- **Distribution plots** for packets and bytes.
- **Countplot** for normal vs anomalous traffic.
- **Heatmap** for feature correlation.

These visualizations helped identify outliers, correlations, and imbalance in class distribution.

## 🧠 Model Training
- Target variable: `Label` (Normal or Anomalous)
- **Features** selected after dropping non-numeric and irrelevant ones.
- **Train/Test Split**: 80% training, 20% testing
- Model Used: **RandomForestClassifier**
- **Evaluation Metrics**:
  - Accuracy Score
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1)

## 🧪 Results
- The model achieved good performance in classifying anomalies.
- Visualizations confirmed class imbalance and helped interpret model results.

## 📊 Sample Visualizations
Plots saved using `plt.savefig()`:
- `lineplot_packets.png`
- `distribution_packets.png`
- `distribution_bytes.png`
- `traffic_label_countplot.png`
- `correlation_heatmap.png`

These can be viewed in the repo under the `/plots` folder (if uploaded).

## 📁 Folder Structure
