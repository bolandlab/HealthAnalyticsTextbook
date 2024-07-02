This folder contains the following files:

1.) **ADR_EHR_diagnosiscodes.csv** This file contains a set of 1,000 fake Electronic Health Records (EHR) patients with ICD 9 & ICD 10 Codes. Each fake patient has 40 diagnostic codes. Entire file is 40,000 rows. The columns in this file are: PATIENT_ID, age_above50, cyp2c9, Code, Version

2.) **phecode_icd9_rolled.csv** This file contains the ICD-9 diagnosis code to PheCode map

3.) **phecode_icd10.csv** This file contains the ICD-10 diagnosis code to PheCode map

4.) **random_set_of_100thousand_delivery_patients_medium.csv** This files contains a set of 100,000 fake Electronic Health Records (EHR) delivery patients. Each fake patient has 2 diagnostic codes. However, some diagnostic codes have multiple codes descriptions. Therefore, this file contains 202,835 rows. The columns in this file are: Code, PATIENT_ID, YEAR, NH_AFAM, NH_WHITE, NH_ASIAN, HISPANIC, WEIGHT_LBS, ENC_AGE_DEC, Version, Description

5.) **icd9_snomed_codemap.csv** This file contains a link between the OMOP or OHDSI CDM concept IDs to those of the ICD-9 diagnosis codes and finally to the SNOMED-CT codes. This can be useful if you are looking to just map those codes using only ICD-9. Typically one would link all local diagnostic codes (typically ICD-9 and ICD-10) to the OHDSI/OMOP CDM concept IDs and then link from there to retrieve the SNOMED-CT codes


