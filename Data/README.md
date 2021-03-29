# Codebook for integrated_protest.csv

Corresponding author: Aida Rahim

March, 2021

The following codebook accompanies the jupyter notebook ’01_Integrate_Datasets_EDA.ipynb’ and organizes the final set of variables by their source file.

### Main datasets:
1. protests in the US (2020-2021): [ACLED Protest Data](https://acleddata.com/special-projects/us-crisis-monitor/)

  * Data file: Protest_US_2020.csv
2. numbers of protesters at each protest event in the US (2020-2021): [Data.World](https://data.world/liz-friedman/us-protests-data-2017-onward)
  * Data file: US_protest_attendees.csv
3. population information (from 2014): [Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/L2GSK6)
  * Data file: BLM_cities.csv

### Variables:

Originally from Protest_US_2020.csv (2020-2021):
* id: unique identifier for each protest event
* date: event date
* month: month event occurred in
* year: year event occurred in
* city: city event occurred in
* state: state event occurred in
* time_precision: numeric code indicating level of certainty of the date coded for the event
* event_type: type of event e.g. protests
* sub_event_type: type of sub-event e.g protest with intervention, or peaceful protest
* actor1 (also actor2): named actor involved in event e.g. protestors
* assoc_actor_1 (also assoc_actor_2): named actor associated with or identifying ACTOR 1 e.g. Students or Labor Group
* type_actor_1 (also type_actor_2): numeric code indicating type of ACTOR1
* interaction: numeric code indicating interaction between types of ACTOR1 and ACTOR2
* notes: Short description of the event
* fatalities: Number of reported fatalities which occurred during the event
* county: county event occurred in
* latitude: latitude of the city
* longitude: longitude of the city
* geo_precision: Numeric code indicating level of certainty of the location coded for the event
* source_x: source of the event report e.g. Daily Freeman, KBJR6, Youtube
* source_scale: the scale (local, regional, national, international) of the source

Originally from US_protest_attendees.csv (2020-2021):
* attendees: number of attendees at each event
* tags: notes on reason for protest
* curated: unclear (from Data.World)
* source_y: source of the even report (from Data.World)
* total_articles: number of articles collected for this event

Originally from BLM_cities.csv (2014):
* totalpop: total population of locality
* povertyrate: poverty rate of locality
* blackpop: total black population of locality
* blackpovertyrate: poverty rate of black population of locality
* asianpop: total asian population of locality
* asianpoverty: poverty rate of asian population of locality
* hispanicpop: total hispanic population of locality
* hispanicpoverty: poverty rate of hispanic population of locality
* whitepop: total white population of locality
* whitepovertyrate: poverty rate of white population of locality
* percentbachelor: percent of population with a bachelor's degree or above
* sqmiles: square milage of locality
* deaths: number of non-vehicular police caused deaths by locality
* deaths_unarmed: deaths subset to unarmed people
* deaths_unarmed_black: deaths subset to unarmed black people
* deaths_armed_black: deaths subset to allegedly armed black people
* deaths_black: deaths subset to black people
* deaths_protestyear: number of non-vehicular police caused deaths by locality
* deaths_protestyear_unarmed: deaths subset to unarmed people
* naacpyears: number of years in which locality had an NAACP chapter, 1912-1977
* mayorpartisanship: D: democrat, R: republican
* blackmayor: dummy variable for black mayor
* dem: unclear (number of democratic voters in locality?)
* rep: unclear (number of republican voters in locality?)
* dem_share: democratic vote share, 2008 presidential election
* pop: estimate of total enrolment of colleges in a locality
* hbcu: number of HBCUs in locality
* hbcu2: dummy for presence of an HBCU in locality
* crime: dummy indicator for being listed in the top 100 highest violent crime cities in 2015
* deathduring: dummy variable for localities with deaths_protestyear_unarmed > 0
* per_ba: percent of population with a bachelor's degree or above
* per_black: black population as percentage of total population
* pop_density: total population over square miles
* collegeenrollpc: total enrollment of colleges in a locality / totalpop
* mayorrep: dummy variable for Republican mayor
* unarmed_deaths_pc: unarmed deaths per 10,000 people
* deaths_pc: deaths per 10,000 people
* unarmed_deaths_black_pc: unarmed black deaths per 10,000 people
* deaths_black_pc: black deaths per 10,000 people
