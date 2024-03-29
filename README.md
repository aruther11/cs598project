# cs598_reproducing_clinical_notes_diagnosis_dl_nlp

In this project I am reproducing the model built in the paper "An empirical evaluation of deep learning for ICD-9 code assignment using MIMIC-III clinical notes" 

Huang, J., Osorio, C., Sy, L. W. (2019).
An empirical evaluation of deep learning
for ICD-9 code assignment using MIMIC-
III clinical notes. Computer Methods and
Programs in Biomedicine, 177, 141–153.

https://doi.org/10.1016/j.cmpb.2019.05.024


--Link to the original paper’s repo (if applicable)

https://github.com/lsy3/clinical-notes-diagnosis-dl-nlp

--Dependencies

Databricks
https://azure.microsoft.com/en-us/free/databricks/search/?&ef_id=Cj0KCQjw1N2TBhCOARIsAGVHQc66dFXl7zdfxdvbEHyBuTTXHQKN_q-ythQEGX18bxiu7VIiqMmpGfQaAhF1EALw_wcB:G:s&OCID=AID2200277_SEM_Cj0KCQjw1N2TBhCOARIsAGVHQc66dFXl7zdfxdvbEHyBuTTXHQKN_q-ythQEGX18bxiu7VIiqMmpGfQaAhF1EALw_wcB:G:s
10.2 ML (includes Apache Spark 3.2.0, GPU, Scala 2.12)
NC6s_v3 - Cluster (DBU / hour: 15 - 45) 

Packages Used within Databricks:

pyspark
sklearn
nltk
teraflow
gensim
pickle
pandas

Unable to generate dependecy yaml through normal python code due to databricks limitations

--Data download instruction

https://physionet.org/content/mimiciii/1.4/



--Preprocessing code:

preprocessing.ipynb

feature_extraction_nonseq.ipynb

feature_extraction_seq.ipynb

word2vec-generator.ipynb

--Training code + command (if applicable)

wordseq_train.ipynb

ml_baseline.ipynb

--Results

LTSM


![image](https://user-images.githubusercontent.com/41799252/167341536-f42a7f5e-4b0b-4a00-879b-be5399ee639e.png)


GRU


![image](https://user-images.githubusercontent.com/41799252/167341578-fac89886-ee61-4786-89d5-19ca0e6956f1.png)
