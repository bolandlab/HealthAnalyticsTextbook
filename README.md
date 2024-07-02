This folder contains the following files:

1.) **ADR_EHR_diagnosiscodes.csv** This file contains a set of 1,000 fake Electronic Health Records (EHR) patients with ICD 9 & ICD 10 Codes. Each fake patient has 40 diagnostic codes. Entire file is 40,000 rows. The columns in this file are: PATIENT_ID, age_above50, cyp2c9, Code, Version

2.) **phecode_icd9_rolled.csv** This file contains the ICD-9 diagnosis code to PheCode map

3.) **phecode_icd10.csv** This file contains the ICD-10 diagnosis code to PheCode map

4.) **random_set_of_100thousand_delivery_patients_medium.csv** This files contains a set of 100,000 fake Electronic Health Records (EHR) delivery patients. Each fake patient has 2 diagnostic codes. However, some diagnostic codes have multiple codes descriptions. Therefore, this file contains 202,835 rows. The columns in this file are: Code, PATIENT_ID, YEAR, NH_AFAM, NH_WHITE, NH_ASIAN, HISPANIC, WEIGHT_LBS, ENC_AGE_DEC, Version, Description

5.) **icd9_snomed_codemap.csv** This file contains a link between the OMOP or OHDSI CDM concept IDs to those of the ICD-9 diagnosis codes and finally to the SNOMED-CT codes. This can be useful if you are looking to just map those codes using only ICD-9. Typically one would link all local diagnostic codes (typically ICD-9 and ICD-10) to the OHDSI/OMOP CDM concept IDs and then link from there to retrieve the SNOMED-CT codes

6.) **matrix_w_netherlands_ALL.csv** This file contains a list of OMOP/OHDSI CDM concept Ids and binary columns indicating if those diagnosis codes were used (i.e., with a frequency of greater than 1,000 patients) at the following sites seattle (seattle_dx column), netherlands (neatherlands_dx column), South Korea (korea_dx column), Taiwan (taiwan_dx column), New York Presbyterian in New York City, NY (cumc_dx column), Mount Sinai Hospital in New York City, NY (mtsinai_dx column), and Vanderbilt University hospital in Nashville, Tennessee (vanderbilt_dx column). Each column is a binary indicator column with a 1 indicating that that condition was found with a prevalence of at least 1,000 patients at the time the queries were run (from 2014-2017), and a 0 indicating that that condition concept id was not found with a prevalence of at least 1,000 patients at that point in time when the query was run.


