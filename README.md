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

#### **Conclusion**
The project aims to visualize and compare the performance of various machine learning models, focusing on precision, recall, and F1 score. By plotting these metrics, you can determine which model performs best overall and assess their strengths and weaknesses.
