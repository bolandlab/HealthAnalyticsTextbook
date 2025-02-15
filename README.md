This folder contains the following files:<br/> 
**SubFolders of Data**<br/> 
1.) **CDC_PLACES_for_GitHub** This subfolder contains files that together make up the CDC PLACES dataset as downloaded in 2024. This is real data and due to size constraints on GitHub is restricted to 31 separate files.


**Fake EHR Datasets**<br/> 
2.) **ADR_EHR_diagnosiscodes.csv** This file contains a set of 1,000 fake Electronic Health Records (EHR) patients with ICD 9 & ICD 10 Codes. Each fake patient has 40 diagnostic codes. Entire file is 40,000 rows. The columns in this file are: PATIENT_ID, age_above50, cyp2c9, Code, Version

3.) **random_set_of_100thousand_delivery_patients_medium.csv** This files contains a set of 100,000 fake Electronic Health Records (EHR) delivery patients. Each fake patient has 2 diagnostic codes. However, some diagnostic codes have multiple codes descriptions. Therefore, this file contains 202,835 rows. The columns in this file are: Code, PATIENT_ID, YEAR, NH_AFAM, NH_WHITE, NH_ASIAN, HISPANIC, WEIGHT_LBS, ENC_AGE_DEC, Version, Description

4.) **random_fakedata_philly_wlatitudeandlongitude_NEW.csv** This file contains a set of fake Electronic Health Records (EHR) pregnancy patients with fake latitude and longitude coordinates that were generated using a fake grid around the center point of Philadelphia (therefore there are non-realistic latitude and longitude points). There is also information on the supposed delivery year, and race/ethnicity of the deliveries. The Race/ethnicity columns consist of NH_AFAM (non-hispanic African American), NH_WHITE (non-hispanic White), HISPANIC (for hispanic), and NH_ASIAN (non-hispanic Asian). Information on the weight of the patient (WEIGHT_LBS), and age (ENC_AGE_DEC) and also if the delivery was the resutl of a multiple birth (MULTIPLE_BIRTH) gestation, a stillbirth (STILLBIRTH), preterm birth (PRETERM) or a Cesearean section delivery (CSECTION). There is also information on the census tract and tract ID (tract, and tractID columns respectively). Note because these data were randomly generated with no baked in correlation, the weights may not correspond realistically with the ages. Also the Race/ethnicity columns may result in a greater or lesser amount of mixed-Race/Ethnicity individuals that one would expect in a real dataset. Each column was created using mainly normal distributions and therefore there is no missingness in this dataset, and it is entirely a randomly generated dataset.

<br/>**Published Datasets**<br/> 
5.) **matrix_w_netherlands_ALL.csv** This file contains a list of OMOP/OHDSI CDM concept Ids and binary columns indicating if those diagnosis codes were used (i.e., with a frequency of greater than 1,000 patients) at the following sites seattle (seattle_dx column), netherlands (neatherlands_dx column), South Korea (korea_dx column), Taiwan (taiwan_dx column), New York Presbyterian in New York City, NY (cumc_dx column), Mount Sinai Hospital in New York City, NY (mtsinai_dx column), and Vanderbilt University hospital in Nashville, Tennessee (vanderbilt_dx column). Each column is a binary indicator column with a 1 indicating that that condition was found with a prevalence of at least 1,000 patients at the time the queries were run (from 2014-2017), and a 0 indicating that that condition concept id was not found with a prevalence of at least 1,000 patients at that point in time when the query was run.

6.) **ALL_NEIGHBORHOOD_COVARIATES_YEARLY_PHILLY.csv** This file contains information from the American Community Survey (ACS) on neighborhood level covariates for Philadelphia. Therefore, it contains census-tract level information for the county of Philadelphia regarding a variety of important covariates from the ACS. It also includes information from the census-tract level that comes from OpenDataPhilly and other resources. This is a real dataset, and was used in several publications, including: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8378638/. 

7.) **BMI_age_standardized_WHO_2014.csv** This file contains information for the entire world from the World Health Organization (WHO) on Body Mass Index (BMI) that is age standardized and from 2014. This is a real dataset, and was used in several publications, including: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 

8.) **DATA_global_fertility_model_182countries_FINAL.csv** This file contains information for the entire world that has been aggregated from multiple sources, including the World Health Organization (WHO) among others. This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 

9.) **FAOSTAT_data_8-22-2017.csv** This file contains information on pesticide usage, which is supposed to be from the entire world, but which we found was lacking several important countries (including the United States of America). It was considered to be used in the following publication, but due to the paucity of data it was not included, but will be included as a learning example in this textbook. Relevant reference: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 

10.) **GDP_global_2010to2016.csv** This file contains information for the entire world on their Gross Domestic Product (GDP) a measure of economic power from WorldBank.com. This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 

11.) **airpollution_global_set1.csv** This file is the first of three files, each labeled set 1, set 2, set 3, respectively that contains information on air pollution for the entire globe. This information originally comes from the World Health Organization (WHO). This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. This is the first set of data (broken into three files due to file constaints on GitHub).

12.) **airpollution_global_set2.csv** This file is the second of three files, each labeled set 1, set 2, set 3, respectively that contains information on air pollution for the entire globe. This information originally comes from the World Health Organization (WHO). This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. This is the second set of data (broken into three files due to file constaints on GitHub).

13.) **airpollution_global_set3.csv** This file is the third of three files, each labeled set 1, set 2, set 3, respectively that contains information on air pollution for the entire globe. This information originally comes from the World Health Organization (WHO). This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. This is the third set of data (broken into three files due to file constaints on GitHub).

14.) **average_yearly_temp_percountry_wiki.csv** This file contains information for the entire world on their average yearly temperature per country. It was obtained from Wikipedia. This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 

15.) **rawdata_CIA_birthrate_2016_cleaned.txt** This file contains information for the entire world on their yearly birth rate in 2016. The dataset was originally developed by the CIA and is freely available. This is a real dataset, and was used in the following publication: https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0207932. 


 
<br/>**Diagnostic Code Maps**<br/> 
16.) **phecode_icd9_rolled.csv** This file contains the ICD-9 diagnosis code to PheCode map

17.) **phecode_icd10.csv** This file contains the ICD-10 diagnosis code to PheCode map

18.) **icd9_snomed_codemap.csv** This file contains a link between the OMOP or OHDSI CDM concept IDs to those of the ICD-9 diagnosis codes and finally to the SNOMED-CT codes. This can be useful if you are looking to just map those codes using only ICD-9. Typically one would link all local diagnostic codes (typically ICD-9 and ICD-10) to the OHDSI/OMOP CDM concept IDs and then link from there to retrieve the SNOMED-CT codes

19.) **CONCEPT_firstset.csv** A subset sample file of concept information to show an example of information that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 

20.) **CONCEPT_secondset.csv** A subset sample file of concept information (the second subset) to show an example of information that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 

21.) **CONCEPT_thirdset.csv** A subset sample file of concept information to show an example of information (the third subset) that would be used in a CONCEPT table for the OHDSI Common Data Model. Because of size constraints this dataset is split into three sub-files, but it is still not complete. If you want the full dataset you must download it directly from the OHDSI website. 


