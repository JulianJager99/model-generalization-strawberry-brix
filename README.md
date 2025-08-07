# Code for "Evaluating Model Generalization for Brix Prediction in Strawberries Using NIR Spectroscopy"

This repository contains the full codebase for the paper "Evaluating Model Generalization for Brix Prediction in Strawberries Using NIR Spectroscopy". It includes training, evaluation, and analysis scripts for a range of predictive models using near-infrared (NIR) spectral data.

The following models are implemented: PLS, irPLS, lwPLS, CNN, BayesConv-CNN, BayesFC-CNN, and SpecTransformer. Each model is trained on spectral inputs to predict Brix values and is evaluated on RMSEP, R², and Practical Accuracy. Inference time analysis is also included to assess computational efficiency.

The `99-posthoc.ipynb` notebook includes all steps performed after obtaining model predictions. This includes constructing datasets for sensitivity analysis (e.g., with added label noise), performing model comparisons using the Model Confidence Set (MCS) procedure, and bootstrap-based comparisons of performance metrics. It also includes correlation analyses between model uncertainty and predictive performance, using both 100 MC and 10 MC forward passes.
