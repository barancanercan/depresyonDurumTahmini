
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
