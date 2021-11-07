## Can Homeless People Improve their Situation?

Predictive Analyses for Homelessness Datathon, 2021

#### Note: some codes have been commented out to keep the cell outputs confidential

### Methodology:

The dataset provided contained 82K entries and 75 variables, encompassing the monitored data for the support of homeless people in __.  Data types included numericals, categoricals and date-times.

Basic Data Cleaning and Exploratory data analysis was performed on a Notebook in a local computer for confidentiality.  Libaries utilized were pandas, numpy, matplotlib, seaborn and sklearn.

The Research Question that I wanted to address was:

##### "Can graduation from the Homeless Support Program be modelled?"

Random Forest Classifer was used for modelling.

### Results

* A significant portion of the 7-hour datathon was spent on cleaning and understanding the dataset.  Some variables were associated and some often had contradicting data points.

* The mean age of homeless clients was 46 +/- 13 years.  The majority was in the program between 0 - 4 years before exiting or graduating. 

![Screen Shot 2021-11-07 at 11 36 53 AM](https://user-images.githubusercontent.com/71532604/140659326-1ef1e0a8-d514-4121-b1a0-af6e6c24f398.png)

* At least half of the homeless people graduated from housing support.

![Screen Shot 2021-11-07 at 11 38 06 AM](https://user-images.githubusercontent.com/71532604/140659370-a72a5b1d-a29e-4afc-930e-06cbe5867803.png)


* Using data for those who Graduated and those who did Not Graduate, modelling was done using Random Forest.  This showed an AUC-ROC score of 97.8% with an F1 score of 95.7%.

![Screen Shot 2021-11-07 at 11 35 55 AM](https://user-images.githubusercontent.com/71532604/140659303-cfa75b0a-feb8-4649-a162-bd0437f1e6a6.png)

### Interpretation:

Given the time and confidentiality constraints associated, the results show that graduating from homelessness is possible and may be facilitated by the cooperation of the client and the housing support.  


### Possible Future Steps:


* Select entries in the categorical variables that can be grouped to make the dataset less sparse after encoding.

* A less-sparse dataset may facilitate determination of coefficients and feature_importances.
