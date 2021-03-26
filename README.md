# Plagiarism-Detector
Simple Plagiarism Detector deployed on AWS.
This is an academic project to predict whether a given answer text is a plagiarized version of the source text. 

The notebooks and Python files provided here demonstrate two different machine learning models that are used to classify a given text as plagiarized or NOT plagiarized. One model uses a custom built neural network performing binary classification on the output of the model. The other notebook uses a linear SVM from Scikit-Learn library. This project assumes some familiarity with Amazon SageMaker, Scikit-learn, Pytorch, and natural language processing methods.

## Hardware Requirement
This project is designed to run in the Amazon Web Services (AWS) cloud environment. 
The Pytorch neural network model is coded to take advantage of a GPU if available, otherwise it will default to using a CPU. For this demonstration a CPU will be adequate.

## Software Requirement
This project requires the use of Amazon's SageMaker provided through AWS. You will need an AWS account to use this service.

An AWS hosted Jupyter Notebook using running Python 3.6 and Pytorch was used to execute this code.

## Code
The main code for this project is provided in `2_Plagiarism_Feature_Engineering.ipynb`, `3_Training_a_Model-Pytorch.ipynb`, and `3_Training_a_Model.ipynb` notebook files. Additional supporting files are also provided in the additional folders.

## Data
The dataset consists of 95 answer-text files and 5 source-text files. This data is a slightly modified version of a dataset created by Paul Clough (Information Studies) and Mark Stevenson (Computer Science), at the University of Sheffield. The data collection and corpus can be found at their university webpage https://ir.shef.ac.uk/cloughie/resources/plagiarism_corpus.html.

## Run
Simply launch a Jupyter Notebook instance using AWS' SageMaker and clone this Git repository `https://github.com/Onestroke1/Sentiment-Analysis-Website.git`.
Running the code in each Jupyter Notebook in the following order `2_Plagiarism_Feature_Engineering.ipynb`, `3_Training_a_Model-Pytorch.ipynb`, and `3_Training_a_Model.ipynb`  will walk you through each step that was done to achieve the final results. 


