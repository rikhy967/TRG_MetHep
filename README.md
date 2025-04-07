# MRI-based radiomics predicts the pathological response of colorectal liver metastases to systemic therapy 


This repository contains data and codes used in our paper entitled "MRI-based radiomics predicts the pathological response of colorectal liver metastases to systemic therapy".

## Codes

The codes are written in Python V.3.9.18 and the following libraries are employed:

* Pandas V.2.2.3
* NumPy V.1.23.5 
* Scikit-learn V.1.3.2
* Optuna V.3.6.1
* Pyradiomics V.3.1.0
* SimpleITK V.2.3.1


## Jupyter Notebooks

Each task of the project has been developed inside the provided jupyter notebook:

* N4BiasField_OtsuMask.ipynb : Perform N4BiasField Correction and Otsu mask extraction
* Histogram_Matching.ipynb: Perform Histogram matching algorithm using center 1 as reference. Histogram matching was computing on N4BiasField corrected images within values of the Otsu mask.
* Feature_extraction.ipynb: Compute Radiomics features on MRI images after Histogram matching on HBP, PVP sequences and inside Ring and Core ROI.
* ML Analysis_radiomica.ipynb: Training and Validation of the machine learning model develope on Radiomics features
