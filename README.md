# LAS_Accuracy

Authors: Nicole Dussault and Will Parker

Project description: Determine the calibration and discrimination of the waitlist and post-transplant survival models used by the LAS, stratified by risk level. Evaluate the overall accuracy of the LAS by comparing a non-parametric estimate of the observed LAS with the predicted LAS.

Inputs: SRTR SAF, lu_alloc files, cand_thor files, tx_lu files, wait_list_baseline_survival and post_transplant_baseline_survival files, lu_alloc_scores

File run order

A. CREATE WAITLIST DATASET

Waitlist_Data_Clean.rmd

B. CREATE POST TRANSPLANT DATASET

Post_Transplant_Data_Clean.rmd

C. PERFORM ANALYSIS

LAS_SumStats.Rmd                                  #Create Table 1
LAS_accuracy_analysis.rmd                         #Run the main analysis

D. SENSITIVITY ANALYSES

LAS_accuracy_analysis_sensitivity.Rmd             #Count "too sick to transplant" as death on the waitlist
LAS_accuracy_analysis_s1000.Rmd                   #Boostrap with 1000 samples
LAS_accuracy_analysis_s100.Rmd                    #Boostrap with 100 samples
