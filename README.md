
# Neural Foundations of Consciousness: Complexity and Machine Learning Analysis

This project investigates the neural underpinnings of consciousness through the application of complexity measures and machine learning techniques. Specifically, it utilizes MEG datasets, complexity measures like Lempel-Ziv (LZ) and state-space entropy (CSER), and models such as multi-layer perceptrons (MLP) to predict various states of consciousness influenced by psychedelic drugs.

## Project Overview

The goal of this project is to explore how psychedelics such as LSD, Ketamine, and Psilocybin affect brain dynamics and consciousness states by:

1. **Computing Complexity Measures**: Calculating Lempel-Ziv complexity (LZ) and Complexity via State Space Entropy Rate (CSER) on MEG data.
2. **Building Machine Learning Models**: Using a Multi-Layer Perceptron (MLP) to classify drugs or predict export values based on complexity measures.
3. **Cross-Validation & Evaluation**: Utilizing grid search and cross-validation techniques to optimize hyperparameters and improve model accuracy.

## Key Notebooks

- **PRIMARY_ANALYSIS_&_ML_PIPELINE.ipynb**: This notebook contains the primary machine learning pipeline, including preprocessing, feature extraction, and building MLP models to classify drugs or predict export values.
- **LZ_CALCULATION.ipynb**: This notebook computes Lempel-Ziv (LZ) complexity values across different channels and drugs.
- **AAL_Groups.txt**: A reference file grouping the Regions of Interest (ROIs) used in the analysis based on the AAL atlas.

## Project Goals

The core objective of the "Neural Foundations of Consciousness" project is to understand how complexity measures derived from MEG data reflect altered states of consciousness under the influence of psychedelics. Specifically:

1. **Lempel-Ziv Complexity (LZ)**: Measures signal diversity and is widely used as a proxy for neural complexity and consciousness.
2. **CSER (Complexity via State Space Entropy Rate)**: Captures the entropy rate within a state-space model, allowing for the analysis of more structured dynamics.
3. **Machine Learning Pipeline**: Predict states of consciousness or other outputs such as export values using complexity features.

## Methodology

1. **Data Preprocessing**:
   - Raw MEG data is processed and cleaned to ensure quality.
   - Data is organized by condition (placebo vs. drug) and by channel (brain region).
   - LZ and CSER complexity measures are computed for each condition, channel, and drug.

2. **Complexity Calculations**:
   - LZ complexity is calculated across multiple channels to gauge signal diversity during different states of consciousness.
   - CSER is computed using state-space models derived from the MEG data, allowing for entropy-based complexity analysis.

3. **Machine Learning Pipeline**:
   - The MLP model is trained on extracted features (e.g., LZ complexity, CSER) to predict conditions such as drug type or export value.
   - Hyperparameter tuning is performed using grid search and randomized search to optimize the model.

4. **Evaluation**:
   - Cross-validation is employed to ensure model generalization.
   - Metrics like Mean Squared Error (MSE), accuracy, and precision are used for evaluation.

## Requirements

To run this project, you will need the following Python libraries:

- **pandas**: For data manipulation
- **numpy**: For numerical operations
- **matplotlib** & **seaborn**: For data visualization
- **scikit-learn**: For building and evaluating machine learning models
- **scipy**: For statistical computations
- **MNE**: For handling MEG data preprocessing

## How to Run

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-repo-url.git
    ```

2. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Notebooks**:
   - Open the notebooks using Jupyter or any other Python IDE.
   - Run the cells in sequence to preprocess data, compute complexity measures, and build machine learning models.
   - Analyze the results using the provided evaluation metrics.

4. **Data**:
   - MEG data files and the complexity measures (LZ and CSER) are used to generate input features for the machine learning models.
   - The `AAL_Groups.txt` file helps categorize ROIs for analysis based on the AAL brain atlas.

## Results

The project demonstrates how complexity measures like LZ and CSER provide meaningful insights into altered states of consciousness under psychedelics. The MLP models successfully classify drugs based on complexity features, shedding light on the neural dynamics of consciousness.

## Future Work

Further exploration can be conducted by:

- Incorporating additional complexity measures such as ACE or SCE.
- Using alternative machine learning models like Random Forests, SVMs, or deep learning architectures.
- Extending the analysis to include more drugs and conditions.

## Conclusion

The "Neural Foundations of Consciousness" project provides a robust pipeline for analyzing MEG data under psychedelics, leveraging complexity measures and machine learning models to understand the dynamic nature of consciousness. Through this project, we aim to uncover the neural correlates of altered states of consciousness.
