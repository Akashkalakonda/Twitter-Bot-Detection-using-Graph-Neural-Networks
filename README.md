# Twitter-Bot-Detection-using-Graph-Neural-Networks
🔍 Project Overview

Social media platforms like Twitter suffer from automated bot accounts that spread spam, misinformation, and fake engagement. Traditional machine learning approaches rely only on user features and often fail to capture network-level behavior.

In this project, I built a Graph Neural Network (GCN)–based system to detect Twitter bots by modeling Twitter as a graph, where users are nodes and interactions are edges. The model leverages both user-level features and network structure to improve bot detection.

🚀 Key Highlights

Implemented Graph Convolutional Networks (GCN) using PyTorch Geometric

Worked with multiple datasets:

Cresci Benchmark Dataset

TwiBot-22 Dataset

Custom Twitter dataset extracted using Twitter API

Built end-to-end pipeline:

Data preprocessing

Graph construction

Model training & evaluation

Achieved ~90% accuracy on TwiBot-22 dataset

🧩 Datasets Used
1. Cresci Dataset

Benchmark dataset for Twitter bot detection

Used for validating GNN performance on structured social data

2. TwiBot-22 Dataset

Large-scale Twitter dataset with:

User metadata (user.json)

Edge relationships (edge.csv)

Ground-truth labels (label.csv)

Suitable for graph-based deep learning

3. Custom Extracted Dataset

Collected using Twitter API (Tweepy)

Streamlit-based GUI for interactive extraction

Created feature matrix and edge index dynamically

System Architecture

Workflow:

Extract user features

Build Twitter interaction graph

Convert graph to PyTorch Geometric format

Train GCN for node-level classification

Evaluate using multiple metrics

🧠 Model Architecture

2-layer Graph Convolutional Network

ReLU activation

Dropout for regularization

Adam optimizer

Negative Log Likelihood Loss

📊 Results (TwiBot-22)

| Metric    | Value      |
| --------- | ---------- |
| Accuracy  | **90.48%** |
| Precision | 40.91%     |
| Recall    | 21.43%     |
| F1-Score  | 28.12%     |

🛠️ Tech Stack

Programming: Python

Deep Learning: PyTorch, PyTorch Geometric

Graph Processing: NetworkX

Data Analysis: Pandas, NumPy, Seaborn

Visualization: Matplotlib

API & Tools: Tweepy, Streamlit
