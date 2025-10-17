# Iris Extended Dataset Exploratory Data Analysis

This notebook performs an extensive exploratory data analysis (EDA) on the Iris Extended Dataset, a modified version of the classic Iris dataset with additional engineered features. The analysis aims to understand the dataset's structure, identify patterns, and prepare the data for potential machine learning tasks, such as classification.

## Dataset
The dataset used in this notebook is located at `/content/drive/MyDrive/ML_Nyberman/iris_extended.csv`. It includes the original Iris features (sepal length, sepal width, petal length, petal width) along with several engineered features related to area, aspect ratio, ratios between sepal and petal dimensions, differences between sepal and petal dimensions, petal curvature, petal texture, leaf area, square roots of areas, and area ratios. It also includes categorical features like `species` and `soil_type`.

## Notebook Structure

The notebook is organized into the following steps:

- **Step I: Display basic information about the dataset**: This section provides an overview of the dataset's dimensions, data types, and descriptive statistics to get a foundational understanding of the data.
- **Step II: Check for missing values**: This step identifies and visualizes any missing values in the dataset.
- **Step III: Visualize the distribution of numerical features**: Histograms and KDE plots are used to visualize the distributions of all numerical features, helping to understand their central tendency, spread, and shape.
- **Step IV: Visualize the distribution of categorical features**: Count plots are used to visualize the distributions of categorical features, showing the frequency of each category.
- **Step V: Explore the relationships between features**: Scatter plots and pair plots are used to visualize the relationships between selected numerical features, revealing potential correlations and clusters.
- **Step VI. Calculate the correlation matrix**: A correlation matrix and heatmap are generated to quantify and visualize the linear relationships between all numerical features.

## Key Findings

- The dataset contains 1200 entries and 21 features with no missing values.
- The dataset includes both numerical (19 features) and categorical (2 features) data types.
- Distributions of numerical features were visualized, showing varying shapes, including some that appear close to normal and others with skewness or multiple peaks.
- The categorical features (`species` and `soil_type`) distributions were visualized, indicating the counts for each category.
- Pair plots revealed strong positive correlations among petal dimensions and distinct clusters likely corresponding to the different species.
- The correlation matrix confirmed strong correlations between various features, especially among those derived from the original measurements (e.g., `sepal_area` and `sepal_area_sqrt`).

## Next Steps

Based on this EDA, potential next steps include:

- **Feature Engineering**: Further creating or refining features to improve model performance.
- **Data Preprocessing**: Scaling numerical features and encoding categorical features in preparation for machine learning models.
- **Model Selection and Training**: Choosing and training appropriate classification models (e.g., for predicting species).
- **Model Evaluation**: Evaluating model performance using relevant metrics.

This notebook provides a solid foundation for further analysis and modeling on the Iris Extended Dataset.

## How to Run the Notebook

1. Clone this repository to your local machine.
2. Ensure you have Google Colab installed or access to a Colab environment.
3. Upload the `iris_extended.csv` dataset to your Google Drive and update the file path in the notebook accordingly.
4. Run the cells sequentially to reproduce the analysis.

## Dependencies

The following libraries are required to run this notebook:

- pandas
- numpy
- matplotlib
- seaborn
- missingno (for visualizing missing values)

These dependencies can be installed using pip.
