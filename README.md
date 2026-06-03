# DataSet_TADPOLE
Generation of a .cmd file containing the CN, MCI, and AD classes, based on TADPOLE data derived from the ADNI study on Alzheimer's disease.

The Jupyter notebook calculates the final dataset from the TADPOLE_D1_D2.csv file and generates the ADNI_3C.csv file by following these steps:
1 - Read the ADNI file TADPOLE_D1_D2
2 - Select the features of interest
3 - Removes records with missing data (NAN)
4 - Reset the index
5 - Return only one instance per patient—retrieve the patient's most recent appointment from the database
6 - Exclude patients with a transition from DEMENTIA to MCI
7 - Excludes patients who have progressed from MCI to dementia
8 - Group and number the CN, MCI, and AD classes
9 - Remove the patient ID and the exam date
10 - Save the resulting file as a CSV
11 - Calculates the number of instances per class
