# Plagiarism-Detector
Simple Plagiarism Detector deployed on AWS.
This is an academic project to predict whether a given answer text is a plagiarized version of the source text. This project introduces the concept of using an n-gram and Longest Common Subsequence (LCS) to determine levels of plagiarism.

The first 2 notebooks `1_Data_Exploration.ipynb` and `2_Plagiarism_Feature_Engineering.ipynb` walk through some simple data exploration followed by feature engineering. The last 2 notebooks demonstrate two different machine learning models that are used to classify a given text as plagiarized or NOT plagiarized. `3_Training_a_Model-Pytorch.ipynb` uses a custom built neural network performing binary classification on the output of the model using Pytorch. The other notebook `3_Training_a_Model.ipynb` uses a linear SVM from the Scikit-Learn library. This project assumes some familiarity with Amazon SageMaker, Scikit-learn, Pytorch, and natural language processing methods.

## Hardware Requirement
This project is designed to run in the Amazon Web Services (AWS) cloud environment. 
The Pytorch neural network model is coded to take advantage of a GPU if available, otherwise it will default to using a CPU. For this demonstration a CPU will be adequate.

## Software Requirement
This project requires the use of Amazon's SageMaker provided through AWS. You will need an AWS account to use this service.

An AWS hosted Jupyter Notebook using running Python 3.6 and Pytorch was used to execute this code.

## Code
The main code for this project is provided in the following notebook files: `1_Data_Exploration.ipynb`, `2_Plagiarism_Feature_Engineering.ipynb`, `3_Training_a_Model-Pytorch.ipynb`, and `3_Training_a_Model.ipynb`. Additional supporting files are also provided in the given folders.

## Data
The dataset consists of 95 answer-text files and 5 source-text files. This data is a slightly modified version of a dataset created by Paul Clough (Information Studies) and Mark Stevenson (Computer Science), at the University of Sheffield. The data collection and corpus can be found at their university webpage https://ir.shef.ac.uk/cloughie/resources/plagiarism_corpus.html.

## Run
Simply launch a Jupyter Notebook instance using AWS' SageMaker and clone this Git repository https://github.com/Onestroke1/Plagiarism-Detector.
Running the code in each Jupyter Notebook in numerical order will walk you through each step that was done to achieve the final results. 


