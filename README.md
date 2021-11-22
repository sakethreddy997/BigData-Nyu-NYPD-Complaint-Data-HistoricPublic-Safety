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
   
