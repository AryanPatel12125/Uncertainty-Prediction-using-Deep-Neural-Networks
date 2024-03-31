##### Disclaimer : This code was developed in Colaboratory unlike my other projects, so this would be having some lines which would not be supported by
##### Jupyter Notebook i.e Anaconda

# Indoor Location Prediction with Uncertainty Estimation

This repository contains the implementation of various models for predicting indoor locations (latitude and longitude) with an emphasis on uncertainty estimation. The models implemented include Bayesian Neural Networks (BNN), Monte Carlo Dropout (MCDropout), and Deep Ensembles. The project demonstrates how to handle uncertainty in predictions, a crucial aspect in critical applications like indoor navigation and location-based services.

## Dataset

The dataset used in this project is the UJIndoorLoc dataset, which provides WiFi fingerprinting data for indoor localization. The dataset includes signal strengths from WiFi access points and the corresponding latitude and longitude of the measurement location.

## Models

### Bayesian Neural Network (BNN)

Implemented using Pyro and Blitz libraries, the BNN model provides a probabilistic approach to neural networks, allowing for direct estimation of prediction uncertainty.

### Monte Carlo Dropout (MCDropout)

MCDropout is implemented as a regular neural network with dropout layers. By keeping the dropout layers active during inference and performing multiple forward passes, we can estimate the uncertainty of the predictions.

### Deep Ensemble

Deep Ensemble involves training multiple independent models and using their predictions to estimate the overall prediction and its uncertainty. This method is simple yet effective in capturing model uncertainty.

## Results

The models are evaluated based on their prediction accuracy and the quality of their uncertainty estimates. The uncertainty estimation is crucial for practical applications, allowing for more informed decision-making under uncertainty.

## Visualization

The repository includes code for visualizing the predictions and their uncertainties. This includes plotting the mean predictions with confidence intervals and the distribution of prediction uncertainties.

## Dependencies

- PyTorch
- Pyro
- Blitz
- NumPy
- Pandas
- Matplotlib
- Seaborn

## Usage

The code is structured as follows:

1. Data loading and preprocessing
2. Model implementation:
   - Bayesian Neural Network
   - Monte Carlo Dropout
   - Deep Ensemble
3. Training and evaluation
4. Uncertainty estimation and visualization

To run the models, simply execute the corresponding Python scripts or Jupyter notebooks.

## Conclusion

This project showcases the importance of uncertainty estimation in machine learning models, particularly in the context of indoor location prediction. By leveraging Bayesian Neural Networks, Monte Carlo Dropout, and Deep Ensembles, we can obtain not only predictions but also measure the confidence in these predictions.

## Contact

For any queries regarding the implementation or the project, feel free to reach out.
