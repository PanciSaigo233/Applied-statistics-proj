# Blood cell differential count discretization modeling predicts survival in adults reporting to the emergency room: a retrospective cohort study

[https://doi.org/10.5061/dryad.dncjsxm5g](https://doi.org/10.5061/dryad.dncjsxm5g)

## Description of the data and file structure

Fille is in .csv (comma separated value) format. Data are listed in a wide dataframe, de-identifyed patient variables are listed in rows by column variables as continuous and discrete. Column titles are abbreviation as listed in the reference article, as follows:
Hemoglobin (Hb), mean red cell volume (MCV), red cell distribution width (RDW), platelet distribution width (PDW), platelet hematocrit (PCT) and absolute count of red blood cells (RBC), white blood cells (WBC), neutrophils (Ne), lymphocytes (Ly), monocytes (Mo), eosinophils (Eo), basophils (Ba), and platelets (PLT),
[1] "Num" case number
[2] "Wave\_I\_II\_off" three groups, based on COVID-19 registered two epidemic surges in Regione Lombardia issued by Italian Health Authority 
[3] "Age" years
[4] "Sex" F female M male 
[5] "ddFUp" days since admission in Emergency Room to follow up or to death date 
[6] "deadTRUE" alive or deceased by logical (dead=TRUE) 
[7] "Eos" eosinophils count in blood sample x10^9/L
[8] "Neu" neutrophils count in blood sample x10^9/L 
[9] "WBC" white blood cells count in blood sample x10^9/L 
[10]"RDW" red cell distribution width in blood sample (%) 
[11] "MCV" mean red cell volume in blood sample (fl) 
[12] "Hb" Hemoglobin in blood sample (g/dL) 
[13] "RBC" red blood cells count in blood sample x10^12/L 
[14] "Lym" lymphocytes count in blood sample x10^9/L 
[15] "Mon" monocytes count in blood sample x10^9/L 
[16] "PLT" platelets count in blood sample x10^9/L 
[17] "PCT" platelet hematocrit in blood sample (%) 
[18] "PDW" platelet distribution width in blood sample (%) 
[19] "Bas" basophils count in blood sample x10^9/L 
[20]"alive0\_dead1" alive or deceased by factor (0 = alive, 1 =dead)) 
[21] "Dischrd0\_Inward1" discharge at home or in- hospital admission to any ward by factor ( 0= discharged at home ; 1= admitted in hospital, any ward) 
[22] "Hb\_tailr" Hemoglobin value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[23] "RDW\_tailr" red cell distribution width discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[24] "RBC\_tailr" red blood cells count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[25] "MCV\_tailr" mean red cell volume value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[26] "WBC\_tailr" white blood cells value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[27] "Neu\_tailr" neutrophils count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[28] "Lym\_tailr" lymphocytes count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[29] "Mon\_tailr" monocyte count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[30] "Eos\_tailr" eosinophil count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[31] "Bas\_tailr" basophils count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[32] "PLT\_tailr" platelets count value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[33] "PCT\_tailr" platelet hematocrit value discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[34] "PDW\_tailr" platelet distribution width discretized by "tailored" log-relative hazard psplines (0=favourable; 1 = unfavorable) 
[35] "Tailr\_score\_sum" sum of unfavorable hemogram values discretized by "tailored" log-relative hazard psplines 
[36] "Tailr\_BCDC\_score" quintiles of sum of discretized by "tailored" log-relative hazard psplines unfavorable hemogram values 
[37] "Tailr\_AgeSex\_InW\_Wave" sum of unfavorable factors (all Tailored 1, age &gt;73yrs, inward admission, in-COVID19 waves)
[38] "Age\_0fav\_1unf" age discretized by maximally selected rank statistic method (0= favourable &lt;=73 yrs; 1 unfavorable &gt;73y)
[39] "HB\_bench" Hemoglobin value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark)
[40] "RDW\_bench" red cell distribution width discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[41] "RBC\_bench" red blood cells count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[42] "MCV\_bench" mean red cell volume value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[43] "WBC\_bench" white blood cells value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[44] "Neu\_bench" neutrophils count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[45] "Lym\_bench" lymphocyte count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[46] "Mon\_bench" monocyte count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[47] "Eos\_bench" eosinophil count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[48] "Bas\_bench" basophils count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[49] "PLT\_bench" platelets count value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[50 "PCT\_bench" platelet hematocrit value discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[51] "PDW\_bench" platelet distribution width discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) 
[52] "Bench\_score\_sum" sum of unfavorable hemogram values discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark)
[53] "Bench\_BCDC\_score" quintiles of sum of discretized by Clinical and Laboratory Standards Institute (CLSI) (benchmark) hemogram values 
[54] "Bench\_AgeSex\_InW\_Wave" sum of unfavorable factors (all Benchmark 1, age &gt;73yrs, inward admission, in-COVID19 waves)

## Code/Software

.csv dataframe can be imported by an extremely wide range of spreadsheet and analysis dedicated software
