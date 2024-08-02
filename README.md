# Investigating Interpretability of Attention-Mechanisms
This project aims to investigate interpretable attention mechanisms by leveraging various types of attention, such as temporal, spatial, and self-attention, within appropriate architectures. The project consists of several sub-projects, about Time-Series Data Analysis, different Attention types, and visualization methods.

---

## 1. Data Preparation and Analysis

Task: Time-Series Forecasting Financial Data
  
<img src="https://github.com/user-attachments/assets/9675ecc1-b654-4b35-8d1d-697740e0dbf6" width=400/>

Understanding the Data: 
- Analyze the daily closing value of the stock index.
- Identify trends, seasonality, and potential anomalies in the data.

Preprocessing: 
- (Clean the data by handling missing values and outliers.)
- Normalize or scale the data for better model performance.

Feature Engineering:
- ?

Visualization: 
- Visualize the raw and processed data to gain insights into its structure and patterns.
- Use tools like matplotlib or seaborn for data visualization.

---

## 2. Attention Types
a. Softness of attention
- Both Bahdanau and Luong attention use soft attention, meaning they compute a weighted average over all input elements
  - Explore Bahdanau attention. Analyze how the alignment scores are computed and used to focus on relevant parts of the input sequence.

  - Examine Luong attention. Compare and contrast the additive vs. multiplicative attention mechanisms used by Bahdanau and Luong attention respectively.

b. Forms of input feature
- Temporal Attention

<img src="https://github.com/user-attachments/assets/f7d095c0-5b45-4a5e-ac26-f857a5b8b05b" width=400/>

RNNs (e.g., LSTMs with Bahdanau or Luong Attention): Implement temporal attention mechanisms in recurrent neural networks to improve time-series forecasting.
Evaluate the performance of attention-augmented RNNs on benchmark time-series datasets.
Investigate the interpretability of the attention weights in understanding temporal dependencies.

- Spatial Attention
CNNs: Apply spatial attention in convolutional neural networks to enhance image recognition and processing.

c. Input representation

- Self Attention
Transformers: Utilize self-attention mechanisms, such as multi-head attention (MHA), in transformer architectures for tasks requiring extensive contextual understanding.

d. Output representation

- Multi-Head Attention

---
## 3. Evaluation and Visualization
a. Model Evaluation:
- Use appropriate metrics to evaluate the performance of models with attention mechanisms, such as accuracy, precision, recall, F1-score, and mean squared error (MSE) for time-series forecasting.

b. Attention Visualization:
- Develop techniques to visualize attention weights for different types of attention mechanisms.
- Create interactive visualizations to demonstrate how attention focuses on different parts of the input data.

c. Interpretability Analysis:
- (Conduct case studies to illustrate the interpretability of models with attention mechanisms.)
- Compare the interpretability of different attention types in various applications.
