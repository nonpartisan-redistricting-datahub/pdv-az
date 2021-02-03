# pdv-az
Partner data validation for Arizona, from VEST 2018. 

## Raw from source

### Accessible files
- File: VEST Florida, 2018
  - Online: https://dataverse.harvard.edu/file.xhtml?persistentId=doi:10.7910/DVN/UBKYRU/CYEKJ4&version=32.0
  - Source: VEST, Harvard Dataverse
  - AWS: `az_2018.zip`
  - Accessed: 2/3/2021
  - Documentation file: 
    - Online: https://dataverse.harvard.edu/file.xhtml?fileId=4366213&version=32.0
    - AWS: `documentation.txt`
    - Accessed: 2/3/2021
- File: Election results, 2018
  - Online: https://azsos.gov/2018-election-information
  - Source: AZ Secretary of State
  - Accessed: 2/3/2021
  - Note: each county supplies its own format, there is a separate file for each county. We will try to use election results processed by MEDSL instead and see if the results are the same. 
- File: Precinct-level shapefile, 2018
  - Online: https://www.kaggle.com/azsecretaryofstate/arizona-statewide-precinct-shapefile?select=az_vtd_2018_new_pima.shp
  - Source: Kaggle, from Garret Archer
  - AWS: `az_vtd_2018_v2.zip`
  - Accessed: 2/3/2021
  - Note: this file is not listed by VEST, but by MGGG. 
- File: Election results, 2018 (cleaned)
  - Online: https://github.com/MEDSL/2018-elections-official
  - Source: MIT Election Data and Science Lab
  - AWS: `precinct_2018.zip`
  - Accessed: 2/3/2021
  - Note: this file is not listed by VEST. 

### Inaccessible files
- File: Precinct-level shapefile used by VEST
  - "Precinct shapefile from Arizona Secretary of State via personal communication."
  - Note: we will try to use the precinct shapefile that MGGG uses, made available on Kaggle by Garret Archer, formerly Senior Elections Analyst with the Arizona Secratary of State and currently a Data Analyst with ABC15 Arizona. See info above. 

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