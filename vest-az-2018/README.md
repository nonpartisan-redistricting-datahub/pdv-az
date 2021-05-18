# pdv-az
Partner data validation for Arizona, from VEST 2018. 

Our final validation report for this dataset is available [here](https://redistrictingdatahub.org/dataset/vest-2018-arizona-precinct-and-election-results/). 

We do not have the raw data sources available on this Github due to file constraints, but we are happy to share them if needed. 

Please reach out to info@redistrictingdatahub.org to reach our support team if you have any questions.

## Raw from source

### Accessible files
- File: VEST Arizona, 2018
  - Online: https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/UBKYRU/CYEKJ4&version=32.0
  - Source: VEST, Harvard Dataverse
  - File name: `az_2018.zip` (available upon request)
  - Accessed: 3/2/2021
  - Previous version of the file is: `az_2018_vest_v1.zip` (vest version 32), accessed 2/3/2021
  - Documentation file: 
    - Online: https://dataverse.harvard.edu/file.xhtml?fileId=4366213&version=33.0
    - AWS: `documentation.txt`
    - Accessed: 2/3/2021
- File: Election results, 2018
  - Online: https://azsos.gov/2018-election-information
  - Source: AZ Secretary of State
  - Accessed: 2/3/2021
  - Note: each county supplies its own format, there is a separate file for each county. We will try to use election results processed by MEDSL instead and see if the results are the same. 
- File: Election results, 2018 (cleaned)
  - Online: https://github.com/MEDSL/2018-elections-official
  - Source: MIT Election Data and Science Lab
  - File name: `precinct_2018.zip` (available upon request)
  - Accessed: 2/3/2021
  - Note: this file is not listed by VEST. 

### Inaccessible files
- File: Precinct-level shapefile used by VEST
  - "Precinct shapefile from Arizona Secretary of State via personal communication."
  - Online: https://www.kaggle.com/azsecretaryofstate/arizona-statewide-precinct-shapefile?select=az_vtd_2018_new_pima.shp
  - Source: Kaggle, from Garret Archer
  - File name: `az_vtd_2018_v2.zip` (available upon request)
  - Accessed: 2/3/2021
  - Note: VEST does not list their precinct shapefile. We will try to use the precinct shapefile that MGGG uses, made available on Kaggle by Garret Archer, formerly Senior Elections Analyst with the Arizona Secratary of State and currently a Data Analyst with ABC15 Arizona. 

## Notes
Offices & parties covered on the VEST file: 
 - USS: U.S. Senate (R,D,G,Write-in)
 - GOV: Governor (R,D,G,WI)
 - SOS: Secretary of State (R,D,WI)
 - ATG: Attorney General (R,D,WI)
 - TRE: Treasurer (R,D,WI)
 - SPI: Superintendent of Public Instruction (R,D,WI)
 - MNI: State Mine Inspector (R,D,WI)

## Processing
`az_vest_2018.ipynb`: validation script & comments for report
