# BigData-Nyu-NYPD-Complaint-Data-HistoricPublic-Safety
This Repo will consist of the work that is done as part of the big data project 

Team Memebrs:-
| Name          |    Net-Id|
| ------------- | ------------- |
| Max Albrecht  |       ma5416  |
| Saketh        |       SP6322  |
| Sanjana       |       lk2849  |



# What did we do with this data ?
1. Data Exploration
2. Data Profiling using openclean
3. Data Cleaning 

### Overview

The moto of this project is to analyse , gain insights of the data , clean the data in the  dataset.
The dataset used (NYPDComplaint Data Historic) includes all crimes reported to the
New York City Police Department (NYPD) from 2006 to the end of last year (2019).


### Field Name & Description:

    'CMPLNT_NUM' (int)                 Complaint Number
    'CMPLNT_FR_DT' (date)              Complaint From Date
    'CMPLNT_FR_TM' (date)              Complaint From Time
    'CMPLNT_TO_DT' (date)              Complaint To Date
    'CMPLNT_TO_TM' (date)              Complaint To Time
    'ADDR_PCT_CD' (int)                Code of Precinct in which the Incident Occured
    'RPT_DT' (date)                    Report Date
    'KY_CD' (int)                      "Key Code": Offense Classification Code (3 digits)
    'OFNS_DESC' (str)                  Offense Description
    'PD_CD' (int)                      PD Code of Offense. More granular than Key Code
    'PD_DESC' (str)                    PD Description of Offense.
    'CRM_ATPT_CPTD_CD' (str)           Whether Crime was Atempted or Completed (values: 'COMPLETED', 'ATTEMPTED')
    'LAW_CAT_CD' (str)                 Level of Offense (values: 'FELONY', 'VIOLATION', 'MISDEMEANOR')
    'BORO_NM' (str)                    Name of Borough in which Incident Occurred
    'LOC_OF_OCCUR_DESC' (str)          Description of where the incident occurred with respect to the premises
                                       (values:'FRONT OF', 'REAR OF', 'OUTSIDE', 'INSIDE', 'OPPOSITE OF')
    'PREM_TYP_DESC' (str)              Description of the type of premises in which the Incident Occurred
    'JURIS_DESC' (str)                 Description of Jurisdiction in which Incident Occurred
    'JURISDICTION_CODE' (int)          Jurisdiction Code
    'PARKS_NM' (str)                   Name of Park in which Incident Occurred, if Applicable
    'HADEVELOPT' (str)                 Name of NYCHA Housing Development in which Incident Occurred, if Applicable
    'HOUSING_PSA' (int)                Housing PSA
    'X_COORD_CD' (int)                 X-coordinate, New York State Plane Coordinate System
    'Y_COORD_CD' (int)                 Y-coordinate, New York State Plane Coordinate System
    'SUSP_AGE_GROUP' (int)             Age Group of Suspect
    'SUSP_RACE' (str)                  Race of Suspect
    'SUSP_SEX' (str)                   Sex of Suspect
    'TRANSIT_DISTRICT' (int)           Transit-District code
    'Latitude' (float)                 Global Latitude of Location where Incident Occurred
    'Longitude' (float)                Global Longitude of Location where Incident Occured
    'Lat_Lon' (str)                    'Latitude' and 'Longitude' together
    'PATROL_BORO' (str)                Patrol Borough
    'STATION_NAME' (str)               Station Name
    'VIC_AGE_GROUP' (int)              Age Group of Victim
    'VIC_RACE' (str)                   Race of Victim
    'VIC_SEX' (str)                    Sex of Victim
    
    
    (Note: some field descriptions were taken from https://www1.nyc.gov/assets/nypd/downloads/pdf/analysis_and_planning/incident_level_data_footnotes.pdf)
    
    
### Thoughts and comments on data

1. CMPLNT_Num =  check weather the column is integer or if it has any other invalid data
2. CMPLNT_FRM_DT = Check if the year is between 2006-2019 
3. CMPLNT_FR_TM =  Validate if the time is in 24 hour format or not
4. CMPLNT_TO_DT = Check if the year is between 2006-2019
5. CMPLNT_TO_TM = Check whether the time is in 24 hour format
6. RPT_DT = Check if the year is between 2006-2019
7. KY_CD = From the data profiling it is clear that this column does not have any kind of invalid or empty values
8. OFNS_DESC = This field can contain empty values as well because this does not look to be a mandatory field and few descriptions tend to have same meaning but with different names , this can be addressed as part of further analysis by grouping them together and make decisions.
9. PD_CD =  Check for empty values and remove them.
10. CRM_ATPT_CPTD_CD =  Values present are COMPLETED , ATTEMPTED and empty values , so change the empty values field to UNKNOWN.
11. LAW_CAT_CD = This Column has values , FELONY, VIOLATION, MISDEMEANOR values so Check if the offence column just consists of following mentioned offences and from profiling of data it is evident that there is no need of any tranformations as the data seems to be perfectly alright
  
   
