# verbose-sniffle
code


**Detailed Explanation for the Code:**

This code is designed to detect and classify various network attacks using multiple machine learning and deep learning models. The implemented models include DBN, SVM, RNN, SNN, and FNN, each trained and evaluated separately. The input data comes from a dataset containing features relevant to different types of network attacks. You can download this dataset from the following link:

[Network Intrusion Dataset - Kaggle](https://www.kaggle.com/datasets/chethuhn/network-intrusion-dataset)

### Workflow:
1. **Data Loading and Preprocessing**:
   - The code loads data from CSV files, combining them into a unified dataset.
   - Key features relevant to network traffic and attacks are extracted, such as the number of forward and backward packets, packet flags, flow speeds, and packet lengths.
   - The data is cleaned to handle missing or invalid values and normalized for consistency using MinMaxScaler.

2. **Model Definitions**:
   - **DBN (Deep Belief Network)**: A layered model based on RBMs (Restricted Boltzmann Machines), extracting features step by step and utilizing Logistic Regression for classification.
   - **SVM (Support Vector Machine)**: A fast algorithm, which reduces data dimensions using PCA and classifies attacks with high efficiency.
   - **RNN (Recurrent Neural Network)**: An optimized deep learning model using LSTMs to capture temporal dependencies in the data.
   - **SNN (Simple Neural Network)**: A simple neural network with optimization techniques like dropout and regularization to prevent overfitting.
   - **FNN (Feedforward Neural Network)**: A more advanced network with multiple layers, suitable for capturing complex data patterns.

3. **Model Training**:
   - Each model is trained using the input data, and techniques like stratified sampling and class balancing are employed to handle imbalanced datasets.
   - The training process records the time taken and the performance metrics for each model.

4. **Evaluation and Metrics**:
   - Each model is evaluated using standard metrics: Accuracy, Precision, Recall, and F1-Score. These metrics provide insights into the models' ability to detect and classify attacks accurately.

5. **Results Visualization**:
   - A table summarizes the performance of all models, while a comparison chart visually highlights the results.
   - The chart illustrates the effectiveness of each model across the defined metrics, making it easy to identify the best-performing model.

### Key Highlights:
- The models are specifically designed to detect attacks such as **DDoS**, **Infiltration**, and **Port Scans**.
- Thanks to the optimized settings, the models achieve exceptional accuracy, typically ranging between **98% and 99%**.
- The code is flexible and allows for easy integration of new data files or adjustments to model parameters.

This project serves as a powerful tool for analyzing and identifying network threats, providing researchers and network security professionals with a highly effective solution for detecting malicious activities with outstanding performance.


Sample Output:

![image](https://github.com/user-attachments/assets/700a9ccf-b747-465b-8b5b-bc7355cf5d1d)
