Name :Muneppa Sai kiran                                                              
Company :CODTECH IT SOLUTIONS                                                                  
ID :CT08DS9789                                                                               
DOMAIN :ARTIFICIAL INTELLIGENCE                                                         


 1. **Loading the Dataset**:
   - The **Iris dataset** is loaded using `load_iris()` from `sklearn.datasets`, which contains features of flowers and their species labels.
   - The dataset is split into features (`X`) and target labels (`y`).

 2. **Data Splitting**:
   - The data is split into **training** (60%) and **testing** (40%) sets using `train_test_split`.

 3. **Model Initialization**:
   - Four different models are initialized for comparison:
     - **Random Forest** (`RandomForestClassifier`)
     - **Support Vector Machine (SVM)** (`SVC`)
     - **K-Nearest Neighbors (KNN)** (`KNeighborsClassifier`)
     - **Logistic Regression** (`LogisticRegression`)
   
 4. **Model Evaluation Function**:
   - A function `evaluate_model()` is defined to:
     - Train each model on the training data.
     - Make predictions on the test data.
     - Calculate various evaluation metrics:
       - **Accuracy**: Overall correctness of the model.
       - **Precision (Weighted)**: Precision calculated as the weighted average.
       - **Recall (Weighted)**: Recall calculated as the weighted average.
       - **F1 Score (Weighted)**: F1 score calculated as the weighted average.
       - **ROC AUC**: If it's a binary classification problem, the ROC AUC score is also calculated. (For multi-class problems, this metric is omitted.)

 5. **Model Evaluation**:
   - Each model is evaluated using the `evaluate_model()` function, and results are stored in a dictionary.
   - The results for each model are then converted into a pandas DataFrame for easier comparison.

 6. **Displaying Results**:
   - The evaluation metrics for all models are displayed in a table.
   - The results are plotted as a **bar chart** using `matplotlib` to visually compare the models' performance.

 Expected Output:
   - **Model Evaluation Table**: The table shows each model's performance based on accuracy, precision, recall, F1 score, and (if applicable) ROC AUC score.
   - **Bar Chart**: A bar chart visualizing the comparison of models across different metrics, helping to quickly identify the best-performing model based on each evaluation criterion.

 Key Points:
   - The workflow provides a **comprehensive evaluation** of different classification algorithms.
   - The results allow comparison across multiple metrics (accuracy, precision, recall, F1 score, and ROC AUC).
   - The Iris dataset is a **multi-class classification problem**, so ROC AUC is not calculated for these models.
   - The **matplotlib plot** provides a **visual comparison** of models, making it easier to analyze the performance of different classifiers.

This code helps identify which model performs best for the given dataset and evaluation metrics.
The output is:
![Screenshot 2024-11-29 190005](https://github.com/user-attachments/assets/b1c2b1d8-99dd-4799-becc-8e6de8048c8c)
