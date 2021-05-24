Practical Data Science Assignment 2

GENERATING A DATA MODEL FOR PREDICTING RECOVERY or DEATH of THE HEART-FAILURE PATIENT.

Author: This data modelling tasks are being completed as a team of 2 members. 

    Syed Nazmul Kabir
    Yanying Xu

This analysis has been conducted using jupiter notebook.
Details of the versions are shown here:

                        jupiter core : 4.6.3
                        jupiter-notebook: 6.1.4
                        ipython: 6.1.4                     

     
The purpose of this analysis is to establish two machine learning models for
predicting survival or death incidents of the heart-failure patients. This analysis is 
addressing a pure classification problem of data-science. While building-up models, the 
analysis also focuses on important features that have strong relationships with the death 
events of the heart-failure patients. So, the analysis will also find out the key factors 
contributing towards increased risk of mortality among heart failure patients.   

Before creating and implementing data models, each attribute in the dataset is explored 
using appropriate visualisations and descriptive statistics. Then the relationship between 
pairs of attributes is identified following the same approach. Finally, two data models are 
selected to train the given dataset according to the findings from the data exploration 
activities. In the report.pdf, a detailed explanation is provided to focus on how the 
models are trained up and how the models are validated.

Files related to this analysis:

         a) heartFailure.ipynb
         b) heart_failure_clinical_records_dataset.csv
         c) README.md
         d) report.pdf

How to Run The Ipynb script:

         Easy way to run the script in anyones's local machine is:

         a)  Download hearFailure.ipynb file and 
             heart_failure_clinical_records_dataset.csv dataset from the source. 
         b)  Upload both files in the same folder of the jupiter notebook.
         c)  Click on heartFailure.ipynb file.
         d)  Press >>  which is just right of kernel restart option. This will 
             ultimately restart the kernel , then re-run the whole notebook.
         e)  Wait for few seconds for completion of the restart of kernel and 
             rerunning the whole notebook. 
         f)  When the running of last cell is completed, the running of whole 
             ipynb script is done.

Major Contents of Assignment2.ipynb:
            
         Three important sections:
         
         1) Data Retrieving and checking
         2) Data exploration
              2.1: Exploration of each attributes
              2.2: Exploration of relationships between pair of attributes.
         3) Data modelling
              3.1: Decision Tree implementation
              3.2: K Nearest Neighbours Implementation
              3.3: K-Fold Cross Validation.

Automation capability:

The ipynb script is  fully capable to run automatically with the further data 
that are in the same format to solve the same classification prediction successfully.
Just need to set the new dataset in the code appropriately and in working repository 
in place of existing data set.
    
