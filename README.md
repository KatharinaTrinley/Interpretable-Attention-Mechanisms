# Investigating the interpretability of attention mechanisms
This project aims to investigate interpretable attention mechanisms by exploiting different types of attention, such as temporal, spatial and self-attention, within appropriate architectures. The project consists of several sub-projects on time-series data analysis, different types of attention, model implementation and visualisation methods.

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

---
---
# Literature Review
### Most relevant literature
1. About Financial Time-Series Analysis


2. About Interpretability of Attention

@misc{rai2024practicalreviewmechanisticinterpretability,
      title={A Practical Review of Mechanistic Interpretability for Transformer-Based Language Models}, 
      author={Daking Rai and Yilun Zhou and Shi Feng and Abulhair Saparov and Ziyu Yao},
      year={2024},
      eprint={2407.02646},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2407.02646}, 
}

4. Model Implementation (RNNs, CNNs, Transformer)
- @inproceedings{10.1145/3604237.3626868,
author = {Cao, Defu and Zheng, Yixiang and Hassanzadeh, Parisa and Lamba, Simran and Liu, Xiaomo and Liu, Yan},
title = {Large Scale Financial Time Series Forecasting with Multi-faceted Model},
year = {2023},
isbn = {9798400702402},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3604237.3626868},
doi = {10.1145/3604237.3626868},
abstract = {Data-driven approaches using deep neural networks have been successful in modeling complex financial time series and generating accurate predictions without requiring extensive domain knowledge. However, most of the existing models that assume independent and identically distributed (i.i.d.) data may not generalize well to novel situations or distributional shifts across or inside financial scenarios. To address this challenge, we introduce an invariant learning-based regularizer with relaxed bounds that expands the range of feasible solutions and mitigates over-convergence issues in Invariant Risk Minimization (IRM). In practice, the regularizer can be incorporated into both linear and nonlinear financial time series forecasting models. Experimental results on real-world large-scale financial datasets show that our proposed method enables more robust and adaptable financial forecasting models, enhancing the overall performance and generalizability of financial forecasting on both in-distribution and out-of-distribution (OOD) samples.},
booktitle = {Proceedings of the Fourth ACM International Conference on AI in Finance},
pages = {472–480},
numpages = {9},
keywords = {Distributional shifts, Financial time series, Forecasting algorithm},
location = {Brooklyn, NY, USA},
series = {ICAIF '23}
}

- @article{10.1007/s11063-022-10767-z,
author = {Kirisci, Melih and Cagcag Yolcu, Ozge},
title = {A New CNN-Based Model for Financial Time Series: TAIEX and FTSE Stocks Forecasting},
year = {2022},
issue_date = {Aug 2022},
publisher = {Kluwer Academic Publishers},
address = {USA},
volume = {54},
number = {4},
issn = {1370-4621},
url = {https://doi.org/10.1007/s11063-022-10767-z},
doi = {10.1007/s11063-022-10767-z},
abstract = {Financial time series forecasting has been becoming one of the most attractive topics in so many aspects owing to its broad implementation areas and substantial impact. Because of this reason in particular recent decades, various kinds of computational intelligence techniques like convolutional neural networks (CNNs) have been used for financial time series forecasting. However, in experiments reported so far, the number of applications of CNNs for the forecasting of financial time series seems quite a few and also in almost all-studies time sequence effect of time series is not preserved on forecasts because of image transformation. From this point of view, in this paper, by aiming to get better forecasting results and avoiding information loss which may occur the process of image transformation, we suggest a new CNN-based forecasting model that can be applied on some time series and, can successfully extract the features of them in the forecasting process. The proposed CNN forecasting model is composed of three convolutional layers and five full connected layers, also to be able to determine the nonlinear relation between input and output Relu and Elu activation functions have also been used. The suggested framework has been applied to some of the most evaluated financial time series, which are Taiwan Stock Exchange Capitalization Weighted Stock Index (TAIEX) and Financial Time Stock Exchange for London stock market data (FTSE). The results have been evaluated on different aspects as an error criterion, a regression analyses and also a visual demonstration. It has been clearly observed that CNN structure has produced outstanding forecasts compared to some other state-of-the-art forecasting tools such as different kinds of ANN, LSTM, fuzzy-based approaches, and some traditional methods.},
journal = {Neural Process. Lett.},
month = {aug},
pages = {3357–3374},
numpages = {18},
keywords = {Convolutional neural network, Financial time series, Forecasting, Deep learning}
}



### more literature

