# Predicting-Fraud-in-Financial-Payment-Services


Trying to recognize and predict fraud in financial transactions is a good example of binary classification analysis. A transaction either is fraudulent, or it is genuine. What makes fraud detection especially challenging is the is the highly imbalanced distribution between positive (genuine) and negative (fraud) classes.

In the analysis I used a synthetic dataset of mobile money transactions. It consists of nearly 6.4 million rows of data divided into five types of transactions; CASH-IN, CASH-OUT, DEBIT, PAYMENT and TRANSFER. Fraud occurs only in two of them; TRANSFER, CASH_OUT. The number of transactions in these types was almost 2.8 million, and the number of fraudulent transactions among them was only c. 8000, making it a truly skewed set of data!

The optimal solution turned out to be a combination of feature-engineering and extreme gradient-boosted decision trees (XGBoost). The predictive power of the model was 0.98, as measured by the area under the precision-recall curve (AUPRC). Crucially, these results were obtained without artificial balancing of the data, such as SMOTE (Synthetic Minority Over-sampling Technique), making this approach suitable to real-world applications
