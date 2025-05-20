# NIH Funding Cuts Drain Training Support for Students and Early Career Scientists

This data journalism project examines trends and patterns in federal data reflecting NIH grant terminations under the Trump admninistration's executive order to eliminate federal funding supporting DEI initiatives.

By: Neela Jain

Date: May 20, 2025

---

## Project Summary

The federal government tracks Department of Health and Human Services (DHHS) grants terminated under the Trump administration’s ‘Ending Radical and Wasteful Government DEI Programs and Preferencing Executive Order’ through the Tracking Accountability in Government Grants System (TAGGS). The transparency tool is maintained by the DHHS Office of Grants which consolidates data submitted to TAGGS by the 12 DHHS operating divisions. The TAGGS data was analyzed to identify grants terminated by the National Institutes of Health (NIH) in an effort to understand how the different grant families (also known as series) of biomedical research funding were impacted by the funding cuts. The results were then applied to active grants data from NIH Report, a federal website providing access to data, reports, and analyses of NIH research activities, to determine the rate of grant terminations per grant family on the basis of active grant volume per grant family.

---

## Data Sources

### TAGGS Data
(Located in 'NIH Terminations Data Analysis 4.30.25/Raw_Data/' folder as both pdf and excel files with keyword 'DOGE')

The TAGGS data was exported on April 30, 2025 and reflects grants terminations between the commencement of terminations of February 28, 2025 and the most recent terminations to date on April 8, 2025. 

### NIH Report Data
(Located in 'NIH Terminations Data Analysis 4.30.25/Raw_Data/' folder as excel file)

The NIH Report data was exported on May 12, 2025 and looks at all active NIH grants to date. (This analysis acknowledges certain inefficiencies owing to the delayed exportation of data from NIH Report following the last known grant terminations on April 8th.) 

---

## Methodology

### Data Cleanup and Analysis
For this project, the TAGGS data was filtered by DHHS agency to narrow results to terminations of NIH grants only. The data was then cleaned to remove duplicate grants based on FAIN data. FAIN (also known as Federal Award Identifier Number) is used to identify grants within federal databases. NIH derives FAIN from the core elements of the NIH grant number as listed on notice of awards.  For example, the FAIN of R01AI654321 consists of the activity code (R01), the code of the NIH institute to which the award is assigned (AI for National Institute of Allergy and Infectious Diseases) and a 6 digit serial number (654321) which represents the federal ID automatically generated for a grant application when submitted to NIH. The data was cleaned once more to isolate the activity code of the FAIN. The activity code was further isolated to include the leading character of the activity code in a separate column named ‘Grant Family.’  The ‘Grant Family’ data identified grants by their class (or series) of NIH funding to help support the parameters of the data analysis.  (For example, ‘Grant Family’ data of ‘F’ represented the Individual Fellowships or ‘F’ series category of NIH funding.) The data was then analyzed to determine the number of grants terminated based on grant family.

Data from NIH Report reflecting all active NIH grants as of May 12th, 2025 was updated in a similar manner to identify grants based on grant family.  The data was then analyzed to determine the number of total active grants based on grant family.

The rate of termination for each grant family was calculated by determining the proportion of terminated grants per grant family by the total number of active grants per grant family inclusive of terminated grants.  

### Analysis Findings and Parameters
The findings focus on grant termination rates for the most commonly awarded grant families.  Thus, the grant termination rate for the ‘C’ grant family which is defined as construction grants providing for the development of a new building, structure or facility, was excluded from the findings’ analysis. The volume of grants in this class of funding ranked at the bottom among all grant families. In addition, the grant termination rate for the ‘O’ grant family (also known as ‘OT’ or ‘Other Transaction’) was excluded as this class of funding represents a unique NIH legal authority other than a grant. Therefore, it does not adhere to the parameters of the analysis. The 'D' and 'S' grant families were also excluded from the finding's analysis as they ranked among the bottom 4 grant families based on number of active awards. Therefore,  six grant families were analyzed in the findings based on volume of active awards prior to termination.

All analysis steps are noted in 'NIH Terminations Data Analysis 4.30.25/Jain_Data_Story_Terminated_NIH_Grants_Analysis_4.30.25/' notebook











