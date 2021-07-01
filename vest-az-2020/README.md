# vest-az-2020

Our final validation report for this dataset is available [here](https://redistrictingdatahub.org/dataset/vest-2020-arizona-precinct-and-election-results/).

We do not have the raw data sources available on this Github due to file constraints, but we are happy to share them if needed. 

Please reach out to info@redistrictingdatahub.org to reach our support team if you have any questions.

## Raw from source

### Accessible files:

- File: VEST AZ 2020 file
   - Date accessed: 7/1/2021
   - Link: https://dataverse.harvard.edu/file.xhtml?fileId=4864722&version=13.0
   - File: `az_2020.zip`
- File: VEST documentation file, 2020
   - Date accessed: 7/1/2021
   - Link: https://dataverse.harvard.edu/file.xhtml?fileId=4863160&version=13.0
   - File: `documentation.txt`
- File: Election results, 2020
  - Date accessed: 6/8/2021
  - Link: https://azsos.gov/2020-election-information
  - File: `Results.Detail_2020General.xml` (available upon request)
  - Note: selected 'Election Results Detail File (zipped .xml file)'
   
### Inaccessible files:
- File: Precinct-level shapefile used by VEST
  - Note from VEST documentation: "Precinct shapefile from Arizona Secretary of State via personal communication"
  - Note: we reached out to Garrett Archer, formerly Senior Elections Analyst with the Arizona Secretary of State and currently a Data Analyst with ABC15 Arizona, because he posted the AZ 2018 precinct shapefile on Kaggle, on 6/14/2021. We have not heard back as of 6/29/2021.   
- File: Precinct-level shapefile for Greenlee County
  - Date accessed: 6/14/2021
  - Link: https://greenleeco.maps.arcgis.com/apps/webappviewer/index.html?id=9bd638cdd2a74d07bce303fe2e77eb3d
  - Note: there is an online arcgis mapping platform with the voting precincts. Called Greenlee County's IT Office at 928-865-5332, the IT Director Vincent Buccellato will be back in office on 6/15 so they will return our call or we will call back then. We emailed Vince on 6/17/2021 but have not heard back as of 6/29/2021. 

## File processing:

`vest-al-2020-validation.ipynb` is the script that is the basis of the validation report
