
# Face Detectives

This project involves detecting facial landmarks and predicting emotional states (such as valence and arousal) using a machine learning model.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Files](#files)
- [Model](#model)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Face Detectives project is designed to analyze facial landmarks and predict emotional states based on those landmarks. The project uses a machine learning model trained to predict emotions, particularly focusing on valence and arousal.

## Installation

To run this project, you'll need to install the required dependencies:

```bash
pip install -r requirements.txt
```

Ensure that you have the necessary libraries such as `numpy`, `tensorflow`, `scikit-learn`, and any other dependencies listed in `requirements.txt`.

## Usage

1. **Facial Landmark Detection**:
   - The notebook uses a pre-trained model to detect facial landmarks. These landmarks are specific points on a face, like the eyes, nose, and mouth.

2. **Feature Engineering**:
   - After detecting and normalizing the landmarks, features are engineered to capture geometric properties that are indicative of emotions.

3. **Model Prediction**:
   - The engineered features are fed into a pre-trained machine learning model to predict emotional states (valence and arousal).
   - The model is loaded from `Models/valence_feature_model.h5`.

### Running the Notebook

To use this notebook:

- Open `face_detectives.ipynb` in Jupyter Notebook or JupyterLab.
- Run the cells sequentially to detect facial landmarks and predict emotions.
- Ensure the model file (`valence_feature_model.h5`) is in the correct path (`/content/Models/`).

## Files

- `face_detectives.ipynb`: Main notebook for detecting facial landmarks and predicting emotions.
- `Models/valence_feature_model.h5`: Pre-trained model used for predicting emotions based on facial features.

## Model

The pre-trained model (`valence_feature_model.h5`) is a neural network trained to predict emotional states (valence and arousal) based on engineered features from facial landmarks.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
