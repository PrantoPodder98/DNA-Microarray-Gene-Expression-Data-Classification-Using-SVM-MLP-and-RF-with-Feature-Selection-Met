# DNA-Microarray-Gene-Expression-Data-Classification-Using-SVM-MLP-and-RF-with-Feature-Selection-Met

## Overview
A DNA microarray (also commonly known as DNA chip or biochip) is a collection of microscopic DNA spots attached to a solid surface. Scientists use DNA microarrays to measure the expression levels of large numbers of genes simultaneously or to genotype multiple regions of a genome.DNA microarray gene expression is being used to detect various forms of diseases. 

In this problem GÜÇKIRAN et al. have classified DNA microarray gene expression data using different classifiers and came to an end with the best one.Using multiple microarray datasets, this paper compares two different methods for classification and feature selection.They used 22 datasets but they didn't combine the datasets here, these are used individually.

We used these 22 datasets and applied on different classification. In our study we found out that LightGBM accuracy is the best among the other classification.


## Contributors
- **Team Members:** [Pranto Podder](https://www.linkedin.com/in/pranto-podder/), [Moumy Kabir](https://www.linkedin.com/in/moumy-kabir-156a0a232/), [Aysha Siddika](https://www.linkedin.com/in/aysha-siddika-577ba5224/), [Tarin Nafisa](https://www.linkedin.com/in/tarin-nafisa-b174031a9/)
- **Course:** Pattern Recognition Project - B.Sc. in Computer Science and Engineering (CSE)
- **Project Duration:** Fall 2021 Trimester (Nov 2021 - Jan 2022)
- **Dataset:** [22 datasets](https://drive.google.com/drive/folders/1_fn0GqGQJAbpqHfLQVDrIeWWSJgIpLmZ?usp=sharing)

## Installing software and files
To do the project, we need to install some softwares and files. In this regard, we will be doing all the implementations in Python language on jupyter notebook. To install jupyter notebook and launch other application and files at first we have to download Anaconda which is free.

Link to Download Anaconda : https://www.anaconda.com/?modal=nucleus-commercial

Guideline for installing Anaconda : https://www.geeksforgeeks.org/how-to-install-anaconda-on-windows/

Once Anaconda is downloaded and installed successfully, we may proceed to download Jupyter notebook.

## Download and Install Jupyter Notebook
Link to download Jupyter using Anaconda : https://docs.anaconda.com/ae-notebooks/4.3.1/user-guide/basic-tasks/apps/jupyter/

More informations : https://mas-dse.github.io/startup/anaconda-windows-install/

Guideline to use Jupyter notebook : https://www.dataquest.io/blog/jupyter-notebook-tutorial/

## Using Google Colaboratory
For implementing the project with no configuration we can use Google Colaboratory as well.

## Installing Python libraries and packages
The required python libraries and packages are,
- pandas
- Numpy
- sklearn
- matplotlib
- seaborn

## Dataset Understanding
* Total 22 datasets. Each of them consists of small sample high dimensional DNA microarray input space, e.g- In borovecki(Instances=31, Features=22283, Classes=2. Each dataset is named by their author
* They used 22 datasets but they didn't combine the datasets here, these were used individually.
* Most of the datasets are for detecting cancer/healthy samples. 
* Also, there are cancer/disease classification datasets.
* In addition to diseases, there are also 3 microarray datasets which are neither disease nor cancer, like aging and environmental effects on DNA.

## State of the Art

* Feature Selection Methods 

Here they have used Relief and LASSO for feature selection methods

**RELIEF:**

This algorithm calculates feature value differences with nearest neighbor pairs.Later, these feature scores are used as important values for the system. High feature score means high importance.

**LASSO:**

LASSO constructs a linear model and penalizes the regression coefficients with L1 distance. Most coefficients are reduced to zero and the remaining inputs are selected.

** Since individual gene counts in microarray data are too many, most informative genes should be selected and used. 
- If we look at the dataset , then you can see that the feature count is so large. It is necessary to reduce the number of features and remove the unnecessary features.
- Feature selection is mandatory for these studies.
- For this selection, they have tried Relief and LASSO feature selection methods.
            
* Classification Methods
After picking informative genes from microarray data, classification is performed   with 

- Support Vector Machines (SVM)
- Multilayer Perceptron Networks (MLP) 
- Random Forest (RF) methods  which are widely used in multiple classification tasks.

* Cross Validation

Cross-validation is an important step to acquire the validity of results. For small sampled datasets like microarray data, it is convenient to use 
Leave-one-out Cross Validation (LOOCV) for the task. 
