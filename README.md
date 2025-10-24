# Machine learning project on Structure-Activity Relationship (SAR) modelling for drug discovery

This project combines the concepts of basic bioinformatics and machine learning to enable prospective drug acitivty prediction of any chemical compound. While bioactivity measures like IC50 determine the potency of the drug to bind and act on its target, drug likeliness factors form a basic set of requirements to be satisfied by any compound before it can be tested for bioactivity. The drug likeliness of chemical compounds is given by Lipinski's rule of five.

## Lipinski's Rule of Five: 
The rule outlines key criteria that a compound should ideally meet to be considered a good candidate for oral bioavailability:

1. Hydrogen Bond Donors: No more than 5 hydrogen bond donors (the total number of nitrogen–hydrogen and oxygen–hydrogen bonds).
2. Hydrogen Bond Acceptors: No more than 10 hydrogen bond acceptors (all nitrogen or oxygen atoms).
3. Molecular Mass: A molecular weight of less than 500 daltons.
4. LogP Value: A calculated octanol-water partition coefficient (logP) that does not exceed 5.


The rule serves as a practical framework for evaluating the physicochemical properties that influence a compound's ADME characteristics. The rule primarily considers passive diffusion as the mechanism for drug absorption. The project performs EDA to clean the data and then calculates molecular descriptors (using RDKit) to quantify the Lipinski factors. After confirming for stastically significant differences between "active" and "inactive" compounds in dataset using these Lipinski factors, we move on to performing ML-based analysis on derived features of each of these compounds to predict their bioactivity. Usually, compounds with very high IC50 values (>10,000 nM) are considered as "inactive" for all practical purposes. 

Post the basic data analysis, the SMILES data are used for derving the PaDEL descriptors of each compound in the dataset. These descriptors act as features for the ML models to predict the activity of the respective compound. Then ML models are build for predicting the IC50 values of each chemical compound in the dataset. The IC50 is the concentration of a drug or compound required to inhibit a biological process by 50%. 

 ## ML models:
 The project demonstrates drug likeliness prediction using four ML models: Random forests, SVM, Linear regression and XGBoost. These are some of the most popular and widely used regression models and  various key prediction metrics like R2 and MSE were computed to evaluate their performance.

## Bibliography:
I would like to thank Prof. Chanin Nantasenamat for his tutorials on ML and drug discovery for helping me understand the basic concepts that enabled me to do this project.
