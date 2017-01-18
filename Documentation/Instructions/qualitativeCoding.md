## St. Louis Street Closure Ordinances
### Qualitative Coding

For every street closure in the city, there should be a corresponding city ordinance that ordered the closure. For analysis purposes, we need to qualitatively code these ordinances into a Stata-friendly format. This is a step by step guide for doing so. 

#### Materials needed:  
1. ordinanceCoding.xlsx (Primary working file - *Available on GitHub* in BarriersLocating -> Excel)
2. waldronCleaned.xlsx (Reference file - *Available on Github* in BarriersLocating -> Excel)
3. The St. Louis City ordinance search engine (https://www.stlouis-mo.gov/government/city-laws/ordinances/)

#### Instructions
The waldronCleaned.xlsx data contains every known street barrier in our database. One by one, we will be entering these barriers into the ordinanceCoding.xlsx spreadsheet.


1. For a given barrier, go to the St. Louis City ordinance search engine and search for that barrier's ordinance number (column G in waldronCleaned.xlsx) **Note: Ordinances prior to 1991 exist only at the Central Branch of the St. Louis Public Library**
2. Click the ordinance and verify that the intersection named in the ordinance actually corresponds with the intersection named in waldronCleaned.xlsx. 
	* If the intersections match in our data and in the ordinance, proceed to enter the appropriate information into the "Matched" sheet in ordinanceCoding.xlsx.
	* If the intersections do not match or the ordinance cannot be found, proceed to enter the barrier and its corresponding information into the "Unmatched" sheet in ordinanceCoding.xlsx
3. Each column corresponds with information in the city ordinance. Use the table below to assist in filling them out. 

#### The following table describes each variable and their appropriate data entries for the "Matched" barriers

| Variable   | Description              | Possible Values       |
| ---------- |:------------------------:| ---------------------:|
| billNum       | Bill Number              |                       |
| alderman      | Alderman who introduced the bill   |   Person's Name         |
| temp          | Is the closure temporary                 |    0=no, 1=yes              |
| duration      | Duration of barrier (months)   |   # of months        |
| justification      | Justification for closure   |   text (i.e. "neighborhood Stability)        |
| emergClause      | Ordianance has an emergency clause   |  0=no, 1=yes        |
| reading1      | Date of first reading   |   MM/DD/YY         |
| refCommit      | Date referred to committee   |   MM/DD/YY         |
|committee     | Committee Type   |   Three letter abbreviation (i.e. STR for street)        |
| subCommit      | Bill referred to sub committee   |   0=no/blank, 1=yes         |
| ammendCommit      | Committee amended the bill   |   0=no/blank, 1=yes         |
| floorAmend     | Floor amendment   |  0=no/blank, 1=yes       |
| floorSub      | Floor subcommittee   |  0=no/blank, 1=yes       |
| perfectn      | TBD   |   MM/DD/YY        |
| passage      | Date passed   |   MM/DD/YY        |
| approved     | Date approved   |   MM/DD/YY, *=blank        |
| veto      | Bill was vetoed   |  0=no/blank, 1=yes       |
| vetoOverule      | Veto overruled   |   0=no, 1=yes, *=N/A        |
| repealOld      | Ordinance repeals old ordinance   |   0=no, 1=yes      |
| repealedOrd      | Ordinance number of repealed ordinance  |  Ordinance Number, *=N/A |
| repealed      | Ordinance is repealed by future ordinance. **Hint: When searching online, any ordinance that repeals an old ordinance should appear as well**   |   0=no, 1=yes       |
| repealedBy      | Ordinance number that repealed ordinance    |   Ordinance Number, *=N/A     |
| keptClosure      | Repealing ordinance kept closure  |  0=no, 1=yes, *=N/A       |
| dateRepealed      | Date ordinance was repealed   |   MM/DD/YY, *=N/A        |



