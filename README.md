
# Python notebooks for simple analysis of CFG arrays

Getting started:
- Open up the notebooks in jupyter
- run 


TLDR
I have wanted to use CFG array data in machine learning but this has been an interesting challenge.
Can all the RF data for all the glycans for a certain array version be used to classify the features of high binders and low binders for a particular disease/lectin ?
I am not sure how to solve this problem but what I have learnt is how to infer which glycans are high binding for a particular array with a fair degree of confidence. This is based on the paper by Cholleti et al. (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3459425/#SD2)

#//There is a fair amount of data but the experiments are not consistent in the way I expected. Often differing concentrations of proteins are used, sometimes there is high error etc. 
#//So how does one choose a set of glycans 

## Notebooks tips
 - when the output is getting out of hand, go to cell | all output | toggle scrolling.
 - when making code changes to notebooks and commiting, please clear all outputs first. 

## Python dependencies
- Download Anaconda python & Install
https://www.continuum.io/downloads
bash Anaconda2-4.0.0-Linux-x86_64.sh
- Make a new environment with rdkit notebook etc
conda create -n pynotes jupyter PIL matplotlib pandas seaborn xlrd scikit-learn
-  To activate this environment, use: # $ source activate pynotes # # To deactivate this environment, use: $ source deactivate #

### installing forgotten dependencies
I previously forgot to install xlrd which is helpful for reading excel files. To do so:
source activate pynotes
conda install xlrd # only use pip if desperate


### additional modifications 
see pip_requirements.txt and conda_env.snapshot for a current view ofthe dependencies (environment needs a retest)
in conda_env.snapshot, any items designated <pip> were installed using pip inside the conda env


# notebooks, pandas and inf resources
http://pyinformatics.blogspot.co.za/2015/05/nested-heatmaps-in-pandas.html
http://chrisalbon.com/python/pandas_normalize_column.html

http://www.analyticsvidhya.com/blog/2016/01/12-pandas-techniques-python-data-manipulation/
http://dataconomy.com/14-best-python-pandas-features/
