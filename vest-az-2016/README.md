# pdv-az
Partner data validation for Arizona, from VEST 2016. 

## Raw from source

### Accessible files
- File: VEST Arizona, 2016
  - Online: https://dataverse.harvard.edu/file.xhtml?fileId=4422286&version=54.0
  - Source: VEST, Harvard Dataverse
  - AWS: `vest_az_2016.zip`
  - Accessed: 3/26/2021
  - Documentation file: 
    - Online: https://dataverse.harvard.edu/file.xhtml?fileId=4441609&version=54.0
    - AWS: `documentation.txt`
    - Accessed: 3/26/2021
- File: Election results, 2016
  - Online: https://apps.azsos.gov/election/2016/General/ElectionInformation.htm
  - Source: AZ Secretary of State
  - Accessed: 
  - Note: each county supplies its own format, there is a separate file for each county. We will try to use election results processed by MEDSL instead and see if the results are the same. 
- File: Election results, 2016 (cleaned)
  - Online: https://github.com/MEDSL/official-precinct-returns
  - Source: MIT Election Data and Science Lab
  - AWS: `2016-precinct-president.zip`, `2016-precinct-senate.zip`
  - Accessed: 3/26/2021
  - Note: this file is not listed by VEST. 

### Inaccessible files
- File: Precinct-level shapefile used by VEST
  - Note from VEST documentation: "Precinct shapefile from Arizona Secretary of State via personal communication."
  - Note: we reached out to Garrett Archer, formerly Senior Elections Analyst with the Arizona Secretary of State and currently a Data Analyst with ABC15 Arizona, because he posted the AZ 2018 precinct shapefile on Kaggle. He emailed us the following file for 2016: 
  - AWS: `pct_2016.zip`
  - Received: 3/23/2021

## Processing
`az_vest_2016.ipynb`: validation script & comments for report
