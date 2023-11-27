# COVID19 Classification from Chest xrays
The objective of this project is to classify xray images and identify the ones that have stronger possibility of COVID vs Normal. Label 0 is assigned if there is no Covid and label 1 is assigned when there is Covid. A quick and accurate detection is very crucial here and a false negative detection (Actually has Covid but prediction as Normal) will prove to be a major disaster even fatal. The classification will be done through custom CNN models as well as Transfer Learning

## Data
Data is provided by Kaggle https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database

A team of researchers from Qatar University, Doha, Qatar, and the University of Dhaka, Bangladesh along with their collaborators from Pakistan and Malaysia in collaboration with medical doctors have created a database of chest X-ray images for COVID-19 positive cases along with Normal and Viral Pneumonia images. This database has 3616 COVID-19 positive cases along with 10,192 Normal, 6012 Lung Opacity (Non-COVID lung infection), and 1345 Viral Pneumonia images and corresponding lung masks. **For this work, only Normal and Covid based xrays are considered**

The data contains various files. The files of concern for this project are

COVID - Folder containing images pertaining COVID xrays\
Normal - Folder containing images pertaining to Normal xrays

## Models and Training

The following models are tried
1. Custom Model with 1e-3 loss
2. Custom Model with 1e-4 loss
3. VGG16 Model with 1e-5 loss
4. VGG16 Model with 5e-6 loss
