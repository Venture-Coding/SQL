Assignment 1 - OMSCS 7641
vrana8@gatech.edu

The folder contains a Jupyter notebook for Assignment 1 code and report for the same.  

To run the code :
•	You need to have Jupyter Notebook installed. (Project Jupyter | Installing Jupyter)
•	You can install it from Anaconda (Jupyter :: Anaconda.org) 
•	Launch it from terminal after opening this folder on your terminal.
•	A sample command looks like :

cd /path/to/this/folder

•	On your terminal or powershell or conda prompt or any other terminal.
•	Open the assignment notebook post launch.
•	Below are libraries used,
	-	Pandas, numpy, seaborn, matploitlib, re, nltk, scikit-learn
•	If any of the imports fails you can install the corresponding libraries using 

pip install library-name 
Or
pip3 install library-name

•	The code starts with importing datasets >> fintech_complaints.csv and adult.csv
Both these files are in the folder.
•	After a little bit of data preprocessing and preparation, we benchmark all selected Classifier models with default parameters on both the datasets.
•	Next we define reusable functions to plot learning_curves, heat_maps and performance scores for each classifier and dataset as and when required.
•	There are 3 datasets, of which 1st and 3rd are primary datasets, while the 2nd dataset of BankNote classification can be ignored.
•	Each model is then passed through GridSearchCV with an exhaustive list of values passed for hyper-parameter tuning.
•	One or two hyperparameters in each model is then selected for further analysis to lot performance scores.
•	Scoring parameter used is F1 score. However, we have a multiclass dataset as well (fintech_complaints). So, scoring used is f1_macro and f1_micro on the basis of literature review and experimentation. 
