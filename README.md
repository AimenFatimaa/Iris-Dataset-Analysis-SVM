# Iris Dataset Analysis and Classification Using SVM

## Project Overview

This project focuses on analyzing the Iris dataset, performing exploratory data analysis (EDA), preprocessing the data, and developing a machine learning classification model using a linear Support Vector Machine (SVM).

The objective is to classify iris flowers into three species based on their sepal and petal measurements.

The project also evaluates the model using training and testing accuracy, precision, and recall.

## Dataset

The Iris dataset contains 150 samples representing three species of iris flowers:

- Setosa
- Versicolor
- Virginica

Each species contains 50 samples.

### Dataset Features

The dataset consists of four input features and one target variable:

| Feature | Description |
|---|---|
| Sepal Length | Length of the sepal in cm |
| Sepal Width | Width of the sepal in cm |
| Petal Length | Length of the petal in cm |
| Petal Width | Width of the petal in cm |
| Species | Target classification variable |

The dataset contains no missing values.

**Dataset Source:** UCI Machine Learning Repository.

For dataset access, see [DATASET.md](DATASET.md).

## Technologies and Libraries

The project uses the following tools and libraries:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab / Jupyter Notebook

## Methodology

### 1. Data Exploration

Initial exploratory data analysis was performed to understand the dataset, examine feature distributions, and investigate relationships between variables.

### 2. Correlation Analysis

A correlation matrix was generated to examine relationships among the numerical features.

The analysis showed strong correlations between petal length and petal width, while sepal width showed relatively weak correlations with other features.

### 3. Outlier Detection

Boxplots were generated to identify potential outliers in the numerical features.

Some outliers were observed, particularly in sepal width. These observations were retained for the analysis.

### 4. Data Preprocessing

The following preprocessing steps were applied:

- **Label Encoding:** The species column was converted into numerical labels (0, 1, and 2).
- **Standardization:** The input features were standardized to have zero mean and unit variance.

### 5. Model Training

A linear Support Vector Machine (SVM) classifier was trained to classify the three Iris species.

The dataset was divided into:

- Training data: 80%
- Testing data: 20%

### 6. Model Evaluation

The model was evaluated using the following performance metrics:

- Accuracy
- Precision
- Recall

## Results and Model Performance

The linear SVM model achieved the following results:

### Training Set Performance

| Metric | Score |
|---|---:|
| Accuracy | 98.33% |
| Precision | 98.37% |
| Recall | 98.37% |

### Testing Set Performance

| Metric | Score |
|---|---:|
| Accuracy | 96.67% |
| Precision | 97.22% |
| Recall | 96.30% |

### Results Discussion

The model achieved high performance on both training and testing data.

The training accuracy was 98.33%, while the testing accuracy was 96.67%. The relatively small difference between these values indicates that the model performed consistently on the two subsets.

The results demonstrate that a linear SVM can effectively classify the three Iris species using their sepal and petal measurements.

## Conclusion and Future Improvements

This project demonstrates a complete machine learning workflow, including exploratory data analysis, data preprocessing, model training, and performance evaluation.

The linear SVM classifier achieved 96.67% testing accuracy, showing strong classification performance on the Iris dataset.

Possible future improvements include:

- Exploring robust scaling or outlier-handling techniques.
- Performing additional feature engineering.
- Experimenting with non-linear SVM kernels, such as the RBF kernel.
- Comparing SVM with other classification algorithms.
- Applying cross-validation for more reliable model evaluation.

