This is the third and final group project for this course.

Description
Part 1 – Data Ingestion & Preprocessing
Data Loading

Acquired the Stanford Sentiment Treebank dataset.
Split into training, validation and test sets with stratified sampling to preserve class balance.
Clearly documented splitting strategy and resulting dataset sizes.
Text Cleaning & Tokenization

Implemented a reusable preprocessing pipeline that handles at least:
HTML removal, lowercasing, punctuation stripping
Vocabulary pruning (e.g., rare words threshold)
Tokenization (character- or word-level)
Exposed this as a function/class so it can be saved and re-loaded for inference.
Feature Extraction

Traditional: Built a TF-IDF vectorizer (or n-gram count) pipeline.
Neural: Prepared sequences for embedding—pad/truncate to a fixed length.
Saved each preprocessor (vectorizer/tokenizer) to disk.
Part 2 – Exploratory Data Analysis (EDA)
Class Distribution

Visualized the number of positive vs. negative reviews.
Computed descriptive statistics on review lengths (mean, median, IQR).
Text Characteristics

Plotted the 20 most frequent tokens per sentiment class.
Generated word clouds (or bar charts) highlighting key terms for each class.
Correlation Analysis

Analyzed whether review length correlates with sentiment.
Presented findings numerically and with at least one visualization.
Part 3 – Baseline Traditional Models
Logistic Regression & SVM

Trained at least two linear models on your TF-IDF features (e.g., logistic regression, linear SVM).
Used cross-validation (≥ 5 folds) on the training set to tune at least one hyperparameter.
Random Forest & Gradient Boosting

Trained two tree-based models (e.g., Random Forest, XGBoost) on the same features.
Reported feature-importance for each and discuss any notable tokens.
Evaluation Metrics

Computed accuracy, precision, recall, F1-score, and ROC-AUC on the held-out test set.
Presented all results in a single comparison table.
Part 4 – Neural Network Models
Simple Feed-Forward

Built an embedding layer + a dense MLP classifier.
Ensured to freeze vs. unfreeze embeddings in separate runs.
Convolutional Text Classifier

Implemented a 1D-CNN architecture (Conv + Pooling) for sequence data.
Justified choice of kernel sizes and number of filters.
Recurrent Model (Optional)

(Stretch) Added an RNN or Bi-LSTM layer and compare performance/time vs. CNN.
Part 5 – Transfer Learning & Advanced Architectures
Pre-trained Embeddings

Retrained one network using pre-trained GloVe (or FastText) embeddings.
Compared results against from-scratch embedding runs.
Transformer Fine-Tuning

Fine-tuned a BERT-family model on the training data.
Clearly outlined training hyperparameters (learning rate, batch size, epochs).
Part 6 – Hyperparameter Optimization
Search Strategy

Used a library (e.g., Keras Tuner, Optuna) to optimize at least two hyperparameters of one deep model.
Described search space and stopping criteria.
Results Analysis

Reported the best hyperparameter configuration found.
Plot validation-loss (or metric) vs. trials to illustrate tuning behavior.
Part 7 – Final Comparison & Error Analysis
Consolidated Results

Tabulated test-set performance for all models (traditional, neural, transfer-learned).
Highlighted top‐performing model overall and top in each category.
Statistical Significance

Performed a significance test (e.g., McNemar’s test) between your best two models.
Error Analysis

Identified at least 20 examples the best model misclassified.
For a sample of 5, provide the raw text, predicted vs. true label, and a short discussion of each error—what linguistic artifact might have confused the model?
