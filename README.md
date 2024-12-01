# Alphabet Soup Charity Funding Predictor

## Overview

This project aims to assist **Alphabet Soup**, a nonprofit foundation, in identifying which charitable organizations are most likely to use funding effectively. Using a deep learning model, the goal was to build a binary classifier to predict the success of funding applications based on various features.

---

## Dataset

The dataset includes information on over 34,000 charitable organizations. Key features include:
- **APPLICATION_TYPE**: Type of application submitted.
- **CLASSIFICATION**: Tax classification of the organization.
- **USE_CASE**: Purpose of funding.
- **INCOME_AMT**: Income classification of the organization.
- **ASK_AMT**: Funding amount requested.

The target variable is **`IS_SUCCESSFUL`**, which indicates if the funding was used effectively (1 = success, 0 = failure).

---

## Model Overview

A deep learning model was built using TensorFlow/Keras. The architecture includes:
- Input Layer: 43 features.
- Hidden Layers:
  - 3 layers with 128, 64, and 32 neurons, respectively.
  - Activation: ReLU.
  - Batch Normalization and Dropout (rate = 0.2) applied to each layer.
- Output Layer: 1 neuron with a sigmoid activation function.

### Optimization Techniques
- **Early Stopping**: Prevented overfitting.
- **Learning Rate Tuning**: Adam optimizer with a learning rate of 0.001.
- **Batch Normalization**: Improved stability and convergence.

---

## Results

- **Loss**: 0.5524
- **Accuracy**: 72.86%

Despite optimization efforts, the target accuracy of 75% was not reached. The model provides a strong foundation for future improvements.
