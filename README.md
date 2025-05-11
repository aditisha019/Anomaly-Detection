# Anomaly-Detection
Anomaly Detection for Data Leakage prevention


A Streamlit-based application using Isolation Forest on the KDD Dataset

🚀 Overview
This app is an interactive web-based tool built using Streamlit that performs unsupervised anomaly detection on network traffic data using the KDD Cup 99 dataset. It leverages the Isolation Forest algorithm to identify unusual or potentially malicious patterns in the data, making it useful for preliminary intrusion detection and network analysis tasks.

📂 Dataset
The app uses the KDDTrain+.txt file from the NSL-KDD dataset, an improved version of the original KDD Cup 99 dataset. It includes 42 columns:

41 features representing various attributes of network traffic

1 label indicating the nature of the connection (normal or an attack)

⚙️ Features
- Automatically assigns column names to raw KDD data

- Preprocesses categorical features using Label Encoding

- Applies Isolation Forest for unsupervised anomaly detection

- Displays anomaly detection results and sample anomalous records

- Simple, clean, and interactive UI using Streamlit

🧪 How It Works
Load Dataset: Reads the raw .txt file without headers.

Preprocess: Converts categorical columns (protocol_type, service, flag) into numeric using LabelEncoder.

Train Model: Trains an IsolationForest with a contamination factor (assumed % of anomalies).

Detect Anomalies: Predicts anomalies and tags each record as either "Normal" or "Anomaly".

Display: Shows anomaly counts and sample data in the web interface.
