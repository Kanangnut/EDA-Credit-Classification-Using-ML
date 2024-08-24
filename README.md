## Fraud Detection System Using Machine Learning

#### **Objective**
The goal of the project is to evaluate and compare the performance of different machine learning models using various metrics. And analyzing both training and testing metrics to determine the effectiveness of each model.

#### **Models Analyzed**
- Logistic Regression
- Random Forest
- Voting Classifier
- Stacking Classifier
- XGBoost
- TensorFlow Neural Network

#### **Metrics**
You are comparing the following metrics:
- Precision
- Recall
- F1 Score

#### **Code Functionality**
1. **`compare_metrics` Function**
   - **Purpose:** This function creates a bar plot comparing various metrics across different models.
   - **Inputs:**
     - `names_models`: A dictionary where keys are model names and values are their corresponding metric values.
     - `metrics`: A list of metrics to be compared.
   - **Output:** Displays a bar plot comparing the specified metrics for each model.

2. **Metric Plotting**
   - The function converts the dictionary of model metrics into a DataFrame and plots them using a bar chart.
   - It includes customizations like colors, bar width, and labels for better visualization.

3. **Plot Customization**
   - **Titles and Labels:** Titles and labels are set for the plot, including axis labels and tick labels.
   - **Bar Labels:** Each bar is annotated with its height to display the exact metric value.

4. **Single Metric Plot**
   - **Purpose:** To visualize a single metric (e.g., recall) across different models for both training and testing sets.
   - **Inputs:**
     - `metric`: The specific metric to plot.
     - `names`: A list of model names.
     - `metrics_tr`: Training metrics for each model.
     - `metrics_ts`: Testing metrics for each model.

5. **Performance Ranking**
   - Based on the metrics, the models are ranked in terms of their performance:
     1. Logistic Regression
     2. Stacking
     3. XGBoost
     4. TensorFlow
     5. Voting
     6. Random Forest

### Conclusion:
The project aims to visualize and compare the performance of various machine learning models, focusing on precision, recall, and F1 score. By plotting these metrics, you can determine which model performs best overall and assess their strengths and weaknesses.

### Key Steps of the Project:

1. **Libraries and Data Handling**: The project utilizes libraries like Pandas and NumPy for data handling, and Matplotlib, Seaborn, and Plotly for data visualization.

2. **Data Preprocessing**: Data is loaded, cleaned (e.g., removing duplicates, handling missing values), and preprocessed using techniques like one-hot encoding for categorical variables and scaling for numerical variables. The dataset is split into training and testing sets.

3. **Exploratory Data Analysis (EDA)**: Detailed exploration of both categorical and numerical data using histograms, box plots, and correlation heatmaps. Insights on data distribution, relationships between variables, and potential feature importance are drawn.

4. **Feature Engineering**: The project performs feature engineering to refine the dataset, such as renaming columns for clarity and converting target variables into appropriate formats (e.g., categorical variables to floats).

5. **Model Development**: Several models are trained:
   - **Logistic Regression**
   - **Random Forest**
   - **Voting Classifier** (combining KNN, Extra Trees, and Logistic Regression)
   - **Stacking Classifier** (with CatBoost and LightGBM)
   - **XGBoost**

6. **Neural Network Approach**: A custom neural network is built using TensorFlow/Keras, including multiple dense layers, dropout layers to prevent overfitting, and callbacks like early stopping to improve model performance.

7. **Evaluation Metrics**: Various evaluation metrics are used to assess model performance:
   - **Precision, Recall, F1-score**
   - **Accuracy, ROC-AUC, and Gini**
   - **Log-loss and Cohen's Kappa**
   - Confusion matrix and Precision-Recall Curves for detailed evaluation.

8. **Model Comparison**: The project compares different models by plotting performance metrics and visualizing misclassifications. It uses metrics like F1-score and ROC curves to evaluate the effectiveness of each model.

9. **Class Imbalance Handling**: To handle imbalanced data, the project incorporates weighted class handling in models like XGBoost and neural networks, ensuring that the model doesn't bias towards the dominant class.

10. **Visualization and Reporting**: Detailed visualizations of model performance, including confusion matrices, ROC curves, precision-recall curves, and performance comparison charts, are presented to showcase model strengths and weaknesses.

### Summary:
This project is an in-depth machine learning analysis showcasing multiple classification techniques applied to a real-world dataset. It explores various modeling approaches, from traditional machine learning models to deep learning, with thorough EDA and model evaluation.
