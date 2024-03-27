# Detect Anomalies in Text Data Using Variational Autoencoder (VAE) in MATLAB® [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=matlab-deep-learning/anomaly-detection-with-text-variational-autoencoder)

This example shows how to detect out-of-distribution text data using a variational autoencoder (VAE).
 

## Overview
VAEs are a neural network architecture composed of two parts:
* An encoder that encodes data in a lower-dimensional parameter space.
* A decoder that reconstructs the input data by mapping the lower-dimensional representation back into the original space.
 
You can use a VAE to detect anomalies in your dataset. To do this, train a VAE on your data. Then, encode and decode a test data point. Compare the output of the decoder with the input data. If the input and output are similar, then the data is in-distribution. If the input and output are dissimilar, then the data is out-of-distribution, or anomalous.

This example includes three steps.
1.	Load and preprocess the text data.
2.	Set up and train the encoder and decoder networks.
3.	Use the VAE to detect anomalies in test data


## Setup
Clone the repository in a local directory. If you would like to use this repository with MATLAB Online, clink [![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=matlab-deep-learning/anomaly-detection-with-text-variational-autoencoder)

The main live script is AnomalyDetectionwithTextusingVAE.mlx. The other .m files are supporting functions for sampling the latent space, projecting and reshaping after sampling from latent space, and initializations of the project and reshape layer. You can either open the .mlx for demo or open the .prj file which will automatically open .mlx file. 

Before running the file, get the data using the following steps: 
- Go to https://www.mathworks.com/help/textanalytics/ug/create-simple-text-model-for-classification.html. 
- Click on the button "Copy Command" on the top right of the page and paste it in MATLAB CLI. This will open the example in the directory where the .csv file is stored. 
- Copy the .csv file from the example, and paste it in the cloned repo.
- If the file is saved in a different location, make sure to change the code that points to it in the .mlx file.

## Required Products
- MATLAB (R2023a or later) 
- Text Analytics Toolbox&trade; (R2023a or later)
- Deep Learning Toolbox&trade; (R2023a or later)

## Contact
Sohini Sarkar, ssarkar@mathworks.com

## License
The license is available in license.txt file in this GitHub repository.

## Community Support
[MATLAB Central](https://www.mathworks.com/matlabcentral)


Copyright 2024, The MathWorks, Inc.



