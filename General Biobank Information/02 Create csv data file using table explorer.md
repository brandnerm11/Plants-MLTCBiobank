# Creating csv data files using Table Explorer App on the RAP

Preparation steps, needed are:

1. Saved cohort under project folder
2. tsv file of said cohort with unix endings  (see "create txt file with unic endings" in this repository). Upload this onto the project with the upload button.

#Running Table explorer step by step

1. Open Tools, select the Table explorer and click run (in case this has not been installed on the RAP yet, install first, clicking install)
2. when window "Run App" opens, leave job name (it only appears in monitor list of current jobs running) and select your project in "Output to", here also an output folder in project can be specific. I found it worked better not specifying this and just clicking "select" (too many errors running for some odd reason)
3. In the inputs sections, select saved cohort, for the file containing field names select the relevant txt files for said cohort
4. under options, specify output prefix (this will be name of csv file)
5. leave output file format as casv, leave coding option as replace
6. for header style, can leave as field name, this will give variable name in form of p12334_i0, if select FIELD-TITLE, it will give meaningful name from cohort browser, e.g. AppleIntakeInstance0 and the dataset is already labelled, rather than FIELD-NAME p1234_i0
  NOTE: This did only work for some files. For some other csv I created it didnt work and all variables from 33 variables were crunched into the ID column.. the field-name however always worked, but needed more work renaming and adding labels (which was quite fast using the data dictionaryI wrote).
8. in advanced options, fill in "participant" for entity. This spans most variables from baseline/assessment centre, clinical biomarkers and nutrition data, however this is a different entity for proteomics data, genomics etc. this can be found out by creating a data dictionary on python. see Bioabank instruction sfor this
9. can leave outputs and other fields alone, then click "START ANALYSis"
10. In runtime options do not need to specify anything, unless maybe spending limit or priority, but cost should be minimal on normal priority, cick "LAUNCH ANALYSIS"!
11. The job is now launched and progress can be seen in the MONITOR section of the RAP, also email is sent upon completion

![Screenshot of how Table Exporter can be filled out to yield desired csv.](/assets/images/03 Table exporter example picture.JPG)
