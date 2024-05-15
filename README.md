
# Depression Status Prediction

This project aims to predict the depression status of individuals using actigraphy data from the Depression Dataset available on Kaggle. The dataset contains CSV files for control and 'condition' groups, providing activity data collected over time. Our goal is to automate the diagnosis of depression based on this activity data.

## Dataset

The dataset is sourced from Kaggle: [The Depression Dataset](https://www.kaggle.com/datasets/arashnic/the-depression-dataset)

## Requirements

The following Python packages are required:

- pandas
- numpy
- scikit-learn

You can install these packages using pip:

```sh
pip install pandas numpy scikit-learn
```

## Project Structure

- `depression_analysis.py`: Contains the code for reading, processing, and analyzing the data, as well as training and evaluating machine learning models.
- `README.md`: Provides an overview of the project, installation instructions, and usage guidelines.
- `depression_dataset/`: Directory containing the downloaded dataset.

## Usage

To run the project, follow these steps:

1. **Clone the repository:**

    ```sh
    git clone https://github.com/barancanercan/depresyonDurumTahmini.git
    cd depresyonDurumTahmini
    ```

2. **Ensure the dataset is placed in the correct directory:**

    Download the dataset from Kaggle and extract it into the `depression_dataset/` directory.

3. **Run the analysis script:**

    ```sh
    python depression_analysis.py
    ```

## Key Findings

1. **Top 10 Happiest Countries:**
    The analysis identifies the top 10 happiest countries, which are Finland, Denmark, Norway, Iceland, Netherlands, Switzerland, Sweden, New Zealand, Austria, and Canada.

2. **Contributing Factors to Happiness:**
    Six factors are found to significantly contribute to happiness:
    - GDP per capita
    - Social support
    - Healthy life expectancy
    - Freedom to make life choices
    - Generosity
    - Perception of corruption

3. **Changes in Happiness Scores:**
    The happiness scores of countries have changed significantly between 2015 and 2019, with some countries experiencing notable increases or decreases.

4. **Correlation Analysis:**
    There is a positive correlation between a country's happiness score and the six contributing factors.

## Model Performance Evaluation

### Random Forest Results:
#### Validation Set:
- Accuracy: 0.6629
- Precision: 0.5926
- Recall: 0.1267
- F1-score: 0.2088

#### Test Set:
- Accuracy: 0.6628
- Precision: 0.5895
- Recall: 0.1297
- F1-score: 0.2127

### SGD Classifier Results:
#### Validation Set:
- Accuracy: 0.5471
- Precision: 0.3535
- Recall: 0.3502
- F1-score: 0.3518

### Comments:
#### Random Forest:
- **Accuracy:** The model's accuracy is approximately 66%, indicating that the model correctly predicts 66% of the instances.
- **Precision:** The precision is around 0.59, meaning that approximately 59% of the positive predictions are actually positive. However, the recall is quite low (0.13), indicating the model's weakness in capturing positive instances.
- **F1-score:** The F1-score is around 0.21, reflecting the imbalance between precision and recall. A low F1-score suggests the overall performance of the model needs improvement.

#### SGD Classifier:
- **Accuracy:** The model's accuracy is approximately 54.7%, which is lower than that of the Random Forest.
- **Precision and Recall:** Both precision and recall values are close to each other, around 0.35. This indicates the model's low rate of correctly predicting and capturing positive instances.
- **F1-score:** The F1-score is around 0.35, indicating that the model performs better than Random Forest in terms of balance between precision and recall, but still has a lower overall accuracy.

### General Evaluation:
#### Model Performance:
- The Random Forest model shows better performance in terms of accuracy (66%), but the imbalance between precision and recall results in a low F1-score.
- The SGD Classifier model has a more balanced precision and recall, but the overall accuracy is lower.

#### Low Recall:
- The low recall values in both models indicate difficulty in capturing positive instances. This can be problematic, especially for identifying critical conditions like depression.

## Contribution

If you wish to contribute to the project, follow these steps:

1. **Fork the repository.**
2. **Make your changes.**
3. **Submit a pull request.**

## License

This project is licensed under the MIT License.

## Acknowledgments

This project is prepared for Data Science Projects by [PatikaDev](https://www.patika.dev/).

![PatikAkademi Logo](https://global-uploads.webflow.com/6097e0eca1e875de53031ff6/6241a5ec363584013b7b1857_Patika%20logo%20(2).png)
