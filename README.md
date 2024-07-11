This folder contains the following files:<br/> 
**Fake EHR Datasets**<br/> 
1.) **ADR_EHR_diagnosiscodes.csv** This file contains a set of 1,000 fake Electronic Health Records (EHR) patients with ICD 9 & ICD 10 Codes. Each fake patient has 40 diagnostic codes. Entire file is 40,000 rows. The columns in this file are: PATIENT_ID, age_above50, cyp2c9, Code, Version

2.) **random_set_of_100thousand_delivery_patients_medium.csv** This files contains a set of 100,000 fake Electronic Health Records (EHR) delivery patients. Each fake patient has 2 diagnostic codes. However, some diagnostic codes have multiple codes descriptions. Therefore, this file contains 202,835 rows. The columns in this file are: Code, PATIENT_ID, YEAR, NH_AFAM, NH_WHITE, NH_ASIAN, HISPANIC, WEIGHT_LBS, ENC_AGE_DEC, Version, Description

3.) **random_fakedata_philly_wlatitudeandlongitude_NEW.csv** This file contains a set of fake Electronic Health Records (EHR) pregnancy patients with fake latitude and longitude coordinates that were generated using a fake grid around the center point of Philadelphia (therefore there are non-realistic latitude and longitude points). There is also information on the supposed delivery year, and race/ethnicity of the deliveries. The Race/ethnicity columns consist of NH_AFAM (non-hispanic African American), NH_WHITE (non-hispanic White), HISPANIC (for hispanic), and NH_ASIAN (non-hispanic Asian). Information on the weight of the patient (WEIGHT_LBS), and age (ENC_AGE_DEC) and also if the delivery was the resutl of a multiple birth (MULTIPLE_BIRTH) gestation, a stillbirth (STILLBIRTH), preterm birth (PRETERM) or a Cesearean section delivery (CSECTION). There is also information on the census tract and tract ID (tract, and tractID columns respectively). Note because these data were randomly generated with no baked in correlation, the weights may not correspond realistically with the ages. Also the Race/ethnicity columns may result in a greater or lesser amount of mixed-Race/Ethnicity individuals that one would expect in a real dataset. Each column was created using mainly normal distributions and therefore there is no missingness in this dataset, and it is entirely a randomly generated dataset.

<br/> 
**Published Datasets**<br/> 
4.) **matrix_w_netherlands_ALL.csv** This file contains a list of OMOP/OHDSI CDM concept Ids and binary columns indicating if those diagnosis codes were used (i.e., with a frequency of greater than 1,000 patients) at the following sites seattle (seattle_dx column), netherlands (neatherlands_dx column), South Korea (korea_dx column), Taiwan (taiwan_dx column), New York Presbyterian in New York City, NY (cumc_dx column), Mount Sinai Hospital in New York City, NY (mtsinai_dx column), and Vanderbilt University hospital in Nashville, Tennessee (vanderbilt_dx column). Each column is a binary indicator column with a 1 indicating that that condition was found with a prevalence of at least 1,000 patients at the time the queries were run (from 2014-2017), and a 0 indicating that that condition concept id was not found with a prevalence of at least 1,000 patients at that point in time when the query was run.

<br/> 
**Diagnostic Code Maps**<br/> 
5.) **phecode_icd9_rolled.csv** This file contains the ICD-9 diagnosis code to PheCode map

6.) **phecode_icd10.csv** This file contains the ICD-10 diagnosis code to PheCode map

7.) **icd9_snomed_codemap.csv** This file contains a link between the OMOP or OHDSI CDM concept IDs to those of the ICD-9 diagnosis codes and finally to the SNOMED-CT codes. This can be useful if you are looking to just map those codes using only ICD-9. Typically one would link all local diagnostic codes (typically ICD-9 and ICD-10) to the OHDSI/OMOP CDM concept IDs and then link from there to retrieve the SNOMED-CT codes

8.) **CONCEPT_firstset.csv** A subset sample file of concept information to show an example of information that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 

9.) **CONCEPT_secondset.csv** A subset sample file of concept information (the second subset) to show an example of information that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 

10.) **CONCEPT_thirdset.csv** A subset sample file of concept information to show an example of information (the third subset) that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 


