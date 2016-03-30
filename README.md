# nyc-schools-water-20160325
Snapshot of New York City public school water test results, retrieved on March 25, 2016

Data is from the [New York City Department of Education](http://schools.nyc.gov/AboutUs/schools/watersafety) which is updating its database as results from 2016 water tests are added. 

Check out our [story and analysis here](http://www.wnyc.org/story/most-new-york-city-schools-have-not-tested-their-water-decade/). 

### Files
* `waterSchools.txt` is a copy of the `waterSchools.txt` [file](http://schools.nyc.gov/Documents/DIIT/waterschools/waterSchools.txt) loaded by the Department of Education [page on water safety](http://schools.nyc.gov/AboutUs/schools/watersafety).   
* `waterPrograms.csv` is a translation of `waterSchools.txt` to `.csv`.
* `waterProgramsInSearch.csv` is a subset of `waterPrograms.csv`. It includes all schools and programs listed in the searchable database by the NYC Department of Education.
* `schools201516.csv` is a list of active New York City public schools in 2015-16 from the [New York City Department of Education](http://schools.nyc.gov/Offices/EnterpriseOperations/DIIT/OOD/default.htm).
* `waterProgramsInSearchFiltered.csv` is a subset of `waterProgramsInSearch.csv`. We've taken out schools whose building code is not listed in `schools201516.csv` and schools that only have Pre-K classes according to the `Grades` field in `schools201516.csv`. This is the file we used for our analysis. 

### Fields in `waterPrograms.csv`, `waterProgramsInSearch.csv` and `waterProgramsInSearchFiltered.csv`
* `location`: name of school
* `dbn`: school's District Borough Number, school code
* `buildingName`: name of building
* `buildingCode`: building code
* `address`: address
* `waterTesting`: whether water testing was performed
* `elevatedResults`: whether any samples from last test had elevated lead levels
* `healthDptProtocolImplemented`: whether the health department protocol was implemented
* `dateLastTested`: year the water was last tested
* `elevatedSamples`: number of elevated samples
* `totalSamples`: total number of samples
* `note`: note about water testing

