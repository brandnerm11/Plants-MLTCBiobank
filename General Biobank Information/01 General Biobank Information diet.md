# How to access dietary information on Biobank
## Food Frequency Questionnaire
(to follow)
## 24-hour diet history

Biobank contains up to five (Instance 0-4) diet histories per person, which has been collected via the validated Oxford WebQ Questionnaire.
It contains both macro- and micronutrients of consumed foods. Foods are also grouped
More information can be found [here](https://biobank.ndph.ox.ac.uk/ukb/ukb/docs/DietWebQ.pdf)


To view the variables in the dataset, these can be explored on the rapic access platform [DNA NEXUS](https://ukbiobank.dnanexus.com/landing) , please log on there. 

To get there

1. On the project landing page after login at press the relevant project (in our case Relationships between plants in our diets (...))
2. Click appxxxx.dataset (Type/Class Dataset Record)
3. Click Data Preview  (this now shows list of participant IDs)
4. Click "add column" to add variables to configure the cohort
5. Click "online follow up" then "Diet by 24hr recall"
6. Various variables can now be selected, if you click add to preview the variable is added to the cohort by participant ID
7. cohorts and specific variables can be configured and saved as a new cohort

NOTE: after 30 columns of variables added this won't be displayed anymore. Furthermore the limit of columns to add to each saved cohort is 200 (including the eid participant ID column). It might therefore be necessary to split cohorts with many variables.

## exporting saved cohorts into data files (csv)

see other readme about creating csv data files using table exporter tool on the RAP 
csv files are needed to access the data with jupyter notebook R, python, Stata etc. 