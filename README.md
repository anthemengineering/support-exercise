SUPPORT Data Science Exercise
=============================

The dataset `support.tsv` contains a random sample of 1000 seriously ill
hospitalized adults from SUPPORT (Study to Understand Prognoses Preferences
Outcomes and Risks of Treatment).

Using the dataset, develop a model to predict *hospital death*.

Please provide any code used to develop your model, a short discussion of your
results, and any assumptions or simplifications made when working with the
data. You may develop a solution in any open source language (e.g. R, Python,
Julia). Please check with us before using proprietary software (e.g. SAS,
Stata, MATLAB).

  Name            Label
  --------------- ------------------------------------------------------------------------
  age             Age
  death           Death at any time up to NDI date (31 Dec 1994)
  sex             Sex
  **hospdeath**   **Death in hospital**
  slos            Date from study entry to discharge
  d.time          Days of follow-up
  dzgroup         Diagnosis group (categorical)
  dzclass         Diagnosis class (categorical)
  num.co          Number of comorbidities
  edu             Years of education
  income          Income (categorical)
  scoma           SUPPORT coma score based on Glasgow D3
  charges         Hospital charges
  totcst          Total RCC cost
  totmcst         Total micro-cost
  avtisst         Average TISS, days 3-25
  race            Race (categorical)
  mean            Mean arterial blood pressure (day 3)
  wblc            White blood cell count (day 3)
  hrt             Heart rate (day 3)
  resp            Respiration (day 3)
  temp            Temperature (celsius) (day 3)
  pafi            PaO2/(0.1 \* FiO2) (day 3)
  alb             Serum albumin (day 3)
  bili            Bilirubin (day 3)
  crea            Serum creatine (day 3)
  sod             Serum sodium (day 3)
  ph              Serum pH (arterial) (day 3)
  glucose         Glucose (day 3)
  bun             Blood urea nitrogen (day 3)
  urine           Urine output (day 3)
  adlp            Number of activities of daily living (ADL) (patient interview) (day 3)
  adls            ADL (surrogate interview) (day 3)
  sfdm2           SUPPORT functional disability measure (ordinal, see table below)
  adlsc           Imputed ADL calibrated to surrogate

  Level       Code                     Meaning
  ----------- ------------------------ -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  1           no(M2 and SIP pres)      Patient lived 2 months to be able to get 2 month interview, and from this interview there were no signs of moderate to severe functional disability.
  2           adl\>=4 (\>= 5 if sur)   Patient was unable to do 4 or more activities of daily living at month 2 after study entry. If the patient was not interviewed but the patient\'s surrogate was, the cutoff for disability was ADL \>= 5.
  3           SIP\>=30                 Sickness Impact Profile total score at 2 months \>= 30
  4           Coma or Intub            Patient intubated or in coma at 2 months
  5           \<2 mo. follow-up        Patient died before 2 months after study entry
  *Missing*   *Missing*                Survived two months, but no patient or surrogate interview.

SUPPORT data were obtained from <http://biostat.mc.vanderbilt.edu/DataSets>.

For additional details about SUPPORT, see "Knaus WA, Harrell FE, Lynn J *et al*.
(1995): The SUPPORT prognostic model: Objective estimates of survival for
seriously ill hospitalized adults. *Annals of Internal Medicine* 122:191-203."
