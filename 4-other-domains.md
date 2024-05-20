# Task 4: Adapt Harmony to other domains

We have developed Harmony initially with psychological instruments in mind.

However we suspect that it could be used for many other domains, such as:

* market research surveys and questionnaires (e.g. "to what extent does this new logo suit our offering / somewhat agree etc?")
* medical history forms
* inclusion and exclusion criteria of clinical studies
* endpoints of clinical studies

Harmony by default tries to assign questionnaire items to mental health categories such as "anxiety" and "depression" by checking the nearest vector match to items in the Mental Health Catalogue. If we make a new "flavour" of Harmony for a different domain, what would we use as our data dictionary in this case?

## Example of medical history forms

I have provided some examples of medical history forms in this folder:

https://drive.google.com/drive/folders/1G8VAWEGasDwm30_sIxCs9uotB0sSV0IC?usp=drive_link 

## Example of exclusion/inclusion criteria

```
DIAGNOSIS AND MAIN CRITERIA FOR INCLUSION AND EXCLUSION:
Eligible patients must meet the following inclusion criteria:
Male or female patients ≥18 years of age at the time of consent
Patient must have been adequately treated with BCG defined as at least one of the following
(FDA 2018):
a. At least five of six doses of an initial induction course plus at least two of three doses of
maintenance therapy
b. At least five of six doses of an initial induction course plus at least two of six doses of a
second induction course
c. A single course of induction BCG can qualify if the patient has T1 high-grade disease at
first evaluation (see 3c)
Patient must be BCG-unresponsive defined as at least one of the following (FDA 2018):
a. Persistent or recurrent CIS alone or with recurrent Ta/T1 disease within 12 months of
completion of adequate BCG therapy. An assessment within 15 months can also qualify
when no assessment was done 12 months after completion of adequate BCG therapy
b. Recurrent high-grade Ta/T1 disease within 6 months of completion of adequate BCG
therapy. An assessment within 9 months can also qualify when no assessment was done
6 months after completion of adequate BCG therapy
c. T1 high-grade disease at the first evaluation following a single course of induction BCG
qualifies (Lerner et al. 2015, Steinberg et al. 2016)
Patient must have, at study entry, NMIBC indicated by 1 or more of the following:
a. Ta or T1 high-grade disease
i. No more than 42 days may elapse between the start of protocol therapy and
complete resection of Ta/T1 papillary disease qualifying the patient for the
study
b. CIS disease
i. Obvious areas of CIS should be fulgurated prior to start of therapy when
indicated
Patient must have no known evidence of concomitant upper tract urothelial carcinoma or
urothelial carcinoma within the prostatic urethra within 6 months of enrollment
Patient must have an Eastern Cooperative Oncology Group performance status ≤2
Patient must have adequate hematologic function, as demonstrated by the following:
a. Hemoglobin level ≥10 g/dL
b. Absolute neutrophil count ≥1.5 x 109/L
c. Platelet count ≥100 x 109/L
Patient must have adequate liver and renal function as demonstrated by the following:
a. Aspartate aminotransferase and alanine aminotransferase each ≤3.0 x upper limit of
normal
b. Total bilirubin ≤1.5 x upper limit of normal, unless prior documentation of Gilbert’s
syndrome in which case, 3.0 mg/dL is allowed
c. Serum creatinine ≤1.5 x upper limit of normal or measured or calculated creatinine
clearance ≥30 mL/min
Female patients of childbearing potential must use maximally effective birth control during the
period of therapy (ie, a combination of 2 regulatory approved methods), must be willing to use
contraception for 1 month after the last study drug infusion, and must have a negative urine or
serum pregnancy test result upon entry into the study. Otherwise, female patients must be
postmenopausal (no menstrual period for a minimum of 12 months) or surgically sterile

10. Male patients who are sexually active must be willing to use a double-barrier contraceptive
method upon study enrollment, during the course of the study, and for 1 month after the last
study drug infusion
11. Patient must be able to understand and sign an informed consent form
12. Patient must be able to comply with protocol requirements, including attendance at required
clinic visits
The presence of any of the following excludes a patient from study enrollment:
1.
Patient has current or previous evidence of muscle invasive (muscularis propria) or metastatic
bladder cancer disease
2. Patient has received investigational therapy for NMIBC
3. Patient has received any therapy for NMIBC within 10 weeks before the start of study treatment
other than surgical resection, 1 dose of chemotherapy, and previous BCG
4. Patient is intolerant to previous BCG treatment in the absence of meeting other criteria for
BCG unresponsiveness and adequate BCG therapy
5. Patient has received external beam radiation therapy for bladder cancer at any time or for any
other condition
6. Patient has an active infection, including urinary tract infection (viral, bacterial, or fungal) and
cystitis
7. Patient has urinary tract signs or symptoms that preclude retention of drug in the bladder; this
does not include anticholinergic drugs
8. Patient is known have tested positive for human immunodeficiency virus (HIV). No HIV testing
is required if patient is not known to have tested positive
9. Patient is female and is pregnant or breastfeeding
10. Patient has any medical, psychological, or social condition or situation that may, in the
investigator’s opinion, make it difficult for the patient to tolerate study medication or comply
with study procedures and other requirements. This includes but is not limited to active
infections, poorly controlled diabetes, uncontrolled cardiac arrhythmia, angina pectoris, or
hypertension
11. Patient has a known presence or history of malignancy of other organ system within the 5 years
before study start, with the exception of non-melanoma skin cancer (eg, basal cell carcinoma or
squamous cell carcinoma of the skin); very low or low-risk prostate cancer (by National
Comprehensive Cancer Network guidelines) defined as prostate-specific antigen <10 ng/dL,
Gleason score ≤6, and clinical stage T1c; or patients who have been disease-free for at least
2 years following stage 1 or 2 cancer
12. Patient is on immunosuppressive therapy or has had a transplant within 12 months before study
start, except for chronic use of corticosteroids (eg, rheumatoid arthritis, asthma, chronic
obstructive pulmonary disease, or any other similarly chronic use of steroids)
13. Patient has any other significant disease that, in the opinion of the investigator, would prevent
study entry
```

## Example of endpoints

```
PRIMARY EFFICACY ENDPOINT:
The primary efficacy endpoint is, in patients with CIS at baseline, the:
• Proportion that achieves a complete response anytime on or after 12 weeks and within the first
48 weeks
Complete response in patients with CIS is defined as at least one of the following:
• Negative cystoscopy and negative (including atypical) urine cytology
• Positive cystoscopy with biopsy-proven benign or low-grade NMIBC and negative cytology
• Negative cystoscopy with malignant urine cytology if cancer is found in the upper tract or prostatic
urethra and random bladder biopsies are negative
The complete response in patients with CIS for this endpoint must be documented on or after the Week 12
response assessment and on or prior to the Week 48 assessment. Duration of complete response in CIS
patients will be calculated from the documented onset of the complete response to the assessment where
the patient no longer meets the definition of complete response. More generally, recurrence is defined as
the reappearance or persistence of high-grade disease or new high-grade disease including CIS.
Recurrence must be biopsy proven. Persistence, appearance, or presence of lower grade disease will not
be considered recurrence.
SECONDARY EFFICACY ENDPOINTS:
The secondary endpoints include the following:
• The incidence of EFS at 48 weeks, where EFS is defined as high-grade recurrence-free survival
(overall population and subgroup of patients with CIS)
• The incidence of EFS at 12, 24, 36, 72, and 96 weeks, where EFS is defined as high-grade
recurrence-free survival (overall population and subgroup of patients with CIS)
• Time to recurrence; recurrence is defined as an EFS event
• The incidence of progression-free survival at 48, 72, and 96 weeks as well as time to progression
estimated using Kaplan-Meir methods. Progression is defined as the development of T2 or greater disease. Sensitivity analyses will also be performed and will include any of the following
as progressions:
o An increase in stage from Ta or CIS to T1, or
o Development of T2 or greater, or
o Lymph node disease, or
o Distant metastasis
Overall survival of patients enrolled in the study at 48, 72, and 96 weeks and survival time
estimated using Kaplan-Meier methods
Changes in quality of life over time, as measured by the European Organization for Research and
Treatment of Cancer Quality of Life Questionnaire (EORTC QLQ-C30; a general questionnaire
for cancer) and the Non-Muscle Invasive Bladder Cancer Questionnaire (QLQ-NMIBC24; a
specific questionnaire for NMIBC disease)
SAFETY ENDPOINT:
The safety endpoint is occurrence of AEs according to CTCAE version 5.0, regardless of relationship to
study medication.
```


## Example clinical trial protocol documents


Here are some clinical trial protocols, which contain inclusion/exclusion criteria and endpoints:

```
https://ClinicalTrials.gov/ProvidedDocs/51/NCT03371251/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/11/NCT04428411/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/14/NCT02861014/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/47/NCT03066947/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/77/NCT02552277/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/53/NCT01462253/Prot_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/22/NCT02255422/Prot_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/88/NCT03266588/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/84/NCT02028884/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/08/NCT04545008/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/94/NCT02691494/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/73/NCT03553173/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/10/NCT04240210/Prot_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/98/NCT02370498/Prot_SAP_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/58/NCT01706458/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/58/NCT04415658/Prot_SAP_005.pdf
https://ClinicalTrials.gov/ProvidedDocs/82/NCT03031782/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/34/NCT03525834/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/09/NCT00842309/Prot_SAP_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/30/NCT02315430/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/09/NCT04646109/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/29/NCT04446429/Prot_SAP_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/35/NCT02684435/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/56/NCT03051256/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/31/NCT02519231/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/68/NCT02644668/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/79/NCT04401579/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/18/NCT02754518/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/94/NCT01928394/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/01/NCT03390101/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/79/NCT03784079/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/09/NCT02281409/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/52/NCT02193152/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/66/NCT02933866/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/66/NCT03219866/Prot_SAP_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/78/NCT03023878/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/25/NCT03182725/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/64/NCT00858364/Prot_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/64/NCT03657264/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/10/NCT00979810/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/80/NCT03196180/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/34/NCT03449134/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/14/NCT04171414/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/20/NCT03597620/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/58/NCT00656058/Prot_ICF_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/98/NCT02386098/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/23/NCT02034123/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/75/NCT02429375/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/33/NCT00130533/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/61/NCT03816761/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/24/NCT04194424/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/96/NCT02287896/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/77/NCT03406377/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/04/NCT01946204/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/39/NCT02342639/Prot_SAP_ICF_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/75/NCT01811875/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/56/NCT02224456/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/50/NCT02620150/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/79/NCT00769379/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/49/NCT03429049/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/12/NCT03016312/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/10/NCT02655510/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/36/NCT03084536/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/81/NCT02252081/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/15/NCT00867815/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/67/NCT01697267/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/96/NCT02829996/Prot_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/01/NCT00536601/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/36/NCT01672736/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/14/NCT02378714/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/87/NCT04798287/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/97/NCT02487797/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/55/NCT03958955/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/39/NCT02514239/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/36/NCT03817736/Prot_002.pdf
https://ClinicalTrials.gov/ProvidedDocs/25/NCT03661125/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/64/NCT02493764/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/37/NCT03153137/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/22/NCT03517722/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/31/NCT02566031/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/50/NCT03781050/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/61/NCT02261961/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/68/NCT04322968/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/76/NCT03722576/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/69/NCT03489369/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/07/NCT02508207/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/14/NCT02374814/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/82/NCT02981082/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/93/NCT02540993/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/74/NCT01381874/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/50/NCT03952650/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/62/NCT04834362/Prot_SAP_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/98/NCT03708198/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/55/NCT01877655/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/73/NCT01990573/Prot_SAP_001.pdf
https://ClinicalTrials.gov/ProvidedDocs/41/NCT03772041/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/80/NCT02669680/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/34/NCT02163434/Prot_SAP_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/30/NCT03018730/Prot_000.pdf
https://ClinicalTrials.gov/ProvidedDocs/57/NCT03938857/Prot_SAP_001.pdf
```

(a script to download them is here: https://github.com/fastdatascience/clinical_trial_risk/blob/main/data/raw_protocols/download_raw_protocols.sh)
