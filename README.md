# LeNet-5 on FashionMNIST with Regularization Techniques

## Overview

This project implements and trains a LeNet-5 model on the FashionMNIST dataset using different regularization techniques to improve generalization. The models compared include:

* **Baseline LeNet-5**: Without any regularization.
* **LeNet-5 with Dropout**: Dropout applied after the first fully connected layer.
* **LeNet-5 with Weight Decay (L2 Regularization)**: Weight decay applied during optimization.
* **LeNet-5 with Batch Normalization**: Batch normalization applied after each convolutional and fully connected layer.

## Files

* The root of the repo is:

  ```
  CNN_FashionMNIST/
  │
  ├── CNN_FashionMNIST.ipynb   
  ├── README.md      
  ├── best_model_dropout.pth       # Best model with dropout
  ├── best_model_BN.pth            # Best model with Batch Normalization
  ├── best_model_weight_decay.pth  # Best model with Weight Decay
  ├── best_model--1.pth            # Base line model
  ├── .git/           
  ├── data/                        # Data folder containing FashionMNIST dataset
  │   ├── train-images-idx3-ubyte.gz
  │   ├── train-labels-idx1-ubyte.gz
  │   ├── test-images-idx3-ubyte.gz
  │   ├── test-labels-idx1-ubyte.gz
  ```

  

* **CNN_FashionMNIST.ipynb**: The notebook that contains the implementation of the LeNet-5 model and variations, training routines, and analysis of results. This notebook has 5 sections as follows. For the last 4 sections, we trained our models without regularization and using 3 different regularization techniques. You can also use codes under the "Test with saved weights" sections to load the weights we trained and do your inference.

  * Data preparation
  * Without regularization
    * Training
    * Test with saved weights

  * With Dropout
    * Training
    * Test with saved weights

  * With Weight Decay
    * Training
    * Test with saved weights

  * With Batch Normalization
    * Training
    * Test with saved weights


## How to Run

**Run the notebook for data preparation** 

* Open `CNN_FashionMNIST.ipynb` in Jupyter or Google Colab.
* Run all cells under the section **Data preparation** 

**Use models with saved weights we trained to do inference**

* Run all cells under "Test with saved weights" sections to load weights from ".pth" files and then do inference.

**If you want to train your own models and save weights** 

* Run all cells under "Training" sections