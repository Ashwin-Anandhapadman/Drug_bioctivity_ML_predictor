# Drug discovery using machine learning 

This project combines the concepts of basic bioinformatics and machine learning to enable drug discovery (or drug likeliness discovery) of any chemical compound. The drug likeliness of chemical compounds is given by 
Lipinski's rule of five.

## Lipinski's Rule of Five: 
The rule outlines key criteria that a compound should ideally meet to be considered a good candidate for oral bioavailability:

1. Hydrogen Bond Donors: No more than 5 hydrogen bond donors (the total number of nitrogen–hydrogen and oxygen–hydrogen bonds).
2. Hydrogen Bond Acceptors: No more than 10 hydrogen bond acceptors (all nitrogen or oxygen atoms).
3. Molecular Mass: A molecular weight of less than 500 daltons.
4. LogP Value: A calculated octanol-water partition coefficient (logP) that does not exceed 5.

The rule serves as a practical framework for evaluating the physicochemical properties that influence a compound's ADME characteristics. The rule primarily considers passive diffusion as the mechanism for 
drug absorption. The project performs EDA to clean the data and then calculates molecular descriptors (using RDKit) to quantify the Lipinski factos.
Then ML models are build for predicting the IC50 values of each chemical compound in the dataset. The IC50 is the concentration of a drug or compound required to inhibit a biological process by 50%. 


I would iike to thank Prof. Chanin Nantasenamat for his tutorials on ML and drug discovery for helping me understand the basic concepts that enabled me to do this project.
