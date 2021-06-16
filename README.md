# Impact-of-Resuscitation-Code-Assignment in the ICU
Impact of Resuscitation code Assignment in the ICU

## What and Why  
Correlation and Descriptive studies.

Problem Definition: Investigating resuscitation code assignment in the intensive care unit is pertinent because revenue is lost in assigning resources to unnecessary resuscitation attempts, especially in cases where do not resuscitate orders have already been procured. Most Patients come to ICU care after a sudden change in health, not planned. Resuscitation code status generally assigned as Full code (FC), until full prognosis done and patients full wishes  from patient or family are known. This is not easy ! Even in AD (advanced directives) cases, difficult to predict whether stabilization will occur, consequently less aggressive code assignment usually doesn`t occur until after entry into the ICU. For patients who transitioned from FC status, to DNR, or to CMO, the last recorded code status might be used. Null hypothesis question: Is there any relationship between medical, familial and social factors in the assignment of resuscitation code?

Null hypothesis question: Is there any relationship between medical, familial and social factors in the assignment of resuscitation code?

## Input
Input: Synthea , synthetic patient generated data, Mimic iv ICU dataset( https://mimic.mit.edu/iv/ ) , inclusion/exclusion criteria, deidentified longitudinal, cross sectional EHR data: 53,423 critical care admissions, 26 tables, 324 variables Charted Events, laboratory measurements (LOINC), over 2 million rows of unstructured data (provider notes)coded with SNOMED CT, ICD-9, ICD-10 and LOINC codes. Unstructured medical notes and structured deidentified EHR data

## Algorithm 
Algorithm: R, SQL, FHIR, Random forest, Logistic Regression, NLP, Apache Ctakes, tokenization, lemmatization, Word2vec, NLP Models based on data from CTAKES and 'treebanks' in 'CoNLL-U' format. 

## Output
Output: Aggregate composite dataset included Unstructured 19642documents, 5682 unique terms, unstructured variables include BM-25/TF-IDF per doc, doc score, Sentiment polarity and Structured 19642 rows of unique patient admission id with variables including length of stay, Subject_id, Gender, Age.yrs, Saps score (14 aggregate mimic variables ), Mortality & Code status. Document level statistics, random forest prediction, correlation matrix. & Regression model predictions.
