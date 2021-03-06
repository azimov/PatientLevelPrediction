PatientLevelPrediction 3.0.15
======================
- improved shiny PLP viewer
- added diagnostic shiny viewer

PatientLevelPrediction 3.0.14
======================
- updated external validate code to enable custom covariates using ATLAS cohorts
- fixed issues with startAnchor and endAnchor


PatientLevelPrediction 3.0.13
======================
- Deprecating addExposureDaysToStart and addExposureDaysToEnd arguments in createStudyPopulation, adding new arguments called startAnchor and endAnchor. The hope is this is less confusing.
- fixed transfer learning code (can now transfer or fine-tune model)
- made view plp shiny apps work when some results are missing

PatientLevelPrediction 3.0.12
======================
- set up testing 
- fixed build warnings

PatientLevelPrediction 3.0.11
======================
- added tests to get >70% coverage (keras tests too slow for travis)
- Fixed minor bugs
- Fixed deep learning code and removed pythonInR dependancy
- combined shiny into one file with one interface

PatientLevelPrediction 3.0.10
======================
- added recalibration using 25% sample in existing models
- added option to provide score to probabilities for existing models
- fixed warnings with some plots


PatientLevelPrediction 3.0.9
======================
Small bug fixes:
- added analysisId into model saving/loading
- made external validation saving recursive 
- added removal of patients with negative TAR when creating population 
- added option to apply model without preprocessing settings (make them NULL)
- updated create study population to remove patients with negative time-at-risk

PatientLevelPrediction 3.0.8
======================
Changes:
- merged in bug fix from Martijn - fixed AUC bug causing crash with big data
- update SQL code to be compatible with v6.0 OMOP CDM
- added save option to external validate PLP


PatientLevelPrediction 3.0.7
======================
Changes:
- Updated splitting functions to include a splitby subject and renamed personSplitter to randomSplitter
- Cast indices to integer in python functions to fix bug with non integer sparse matrix indices

PatientLevelPrediction 3.0.5
======================

Changes:
- Added GLM status to log (will now inform about any fitting issue in log)
- Added GBM survival model (still under development)
- Added RF quantile regression (still under development)
- Updated viewMultiplePlp() to match PLP skeleton package app
- Updated single plp vignette with additional example 
- Merge in deep learning updates from Chan

PatientLevelPrediction 3.0.4
======================

Changes:
- Updated website

PatientLevelPrediction 3.0.3
======================

Changes:
- Added more tests
- test files now match R files

PatientLevelPrediction 3.0.2
======================

Changes:
- Fixed ensemble stacker 

PatientLevelPrediction 3.0.1
======================

Changes:
- Using reticulate for python interface 
- Speed improvements
- Bug fixes