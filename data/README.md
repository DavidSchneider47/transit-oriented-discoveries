# Metadata for NTD Fixed Guideway Stations

## File Description
- **File Name**: NTD Fixed Guideway Stations.csv
- **Creation Date**: January 2024
- **Data Source**: National Transit Database, 2022 Facilities Inventory.  https://www.transit.dot.gov/ntd/data-product/2022-annual-database-facility-inventory. Data reported by transit agencies in 2022 and published by FTA in November 2023. More information on the NTD can be found at https://www.transit.dot.gov/ntd. 

## Purpose
This dataset contains information on fixed guideway transit stations reported to the National Transit Database, including selected geographic information, including lon/lat coordinates, and information about the transit mode served, station configuration, year built and other information. It also includes a category for each transit agency created by David Schneider (not included in the NTD publication). See additional notes for more information. 

## Column Definitions
1. **NTD ID**: NTD identification number, a unique number assigned to each NTD reporter. 

2. **Agency Name**: The name of the NTD reporter. 

3. **Primary Mode Served**: The system for carrying transit passengers described by specific right-of-way (ROW), technology and operational features that the facility serves. See additional notes for definitions. 

4. **Facility ID**: A five-digit identifying number for each agency used in the current NTD system.

5. **Facility Type**: A category for each facility representing the facility’s relationship to other surface transportation elements. . See additional notes for category definitions.

6. **Facility Name**: The name of the facility provided by the NTD reporter. 

7. **Street Address**: The address of the facility provided by the reporter or derived from the lon/lat information when an address was not provided. 

8. **City** The city that the facility is located in provided by the NTD reporter or derived from the lon/lat information when an address was not provided. 

9. **State**: The state that the facility is located in provided by the NTD reporter or derived from the lon/lat information when an address was not provided. 

10. **Zip Code**: The zip code that the facility is located in provided by the NTD reporter or derived from the lon/lat information when an address was not provided. 

11. **Latitude**: The facility latitude derived from the full address.

12. **Longitude**:The facility longitude derived from the full address.

13. **Square Feet**: The square feet of the facility provided by the NTD reporter. .

14. **Section of a Larger Facility**: Whether or not the facility is part of a larger facility. 

15. **Year Built or Constructed as New**: The year the station was built or renovated, provided by the NTD reporter. 

16. **full address**: The combined street address, city, state, and zip code of the facility, either submitted by the NTD reporter or geocoded from the lon/lat coordinates if not submitted by the reporter. 

17. **County**:The county the facility is located in, derived form the full address.

18. **Category**: A number from 1-6 corresponding to the system definition.

19. **Definition**: The names of the six categories created for the transit systems in the data set. See additional notes for definitions. 

## Usage Instructions
- This dataset excludes 88 stations from the 2022 Facilities Inventory whose longitude and latitude coordinates were found to be inaccurate. A list of these facilities is published separately. See Jupyter Notebook #1 NTD_Data_Cleaning.ipynb for additional information on how this data was derived.

## Additional Notes
- Additional information on primary modes served:

--Heavy Rail: An electric railway that operates service in exclusive right of way.

--Light Rail: An electric railway that operates in mixed traffic or intersects with roadways at grade crossings.

--Streetcar Rail: Systems predominantly operate routes on streets in mixed traffic. 

--Bus Rapid Transit: A bus system that offers 50 percent of its route in a separate right-of-way (ROW) dedicated for transit use during peak period

--Commuter Rail: An electric- or diesel-propelled railway for urban passenger train service consisting of local travel which operates between a central city and outlying areas

--Hybrid Rail: Systems primarily operate routes on the national system of railroads but do not operate with the characteristics of Commuter Rail (i.e. shorter trips but on freight rail tracks).

--Additional information on facility type:

--Elevated fixed guideway station: stations located above grade built on a viaduct, a steel or concrete structure, or on retained fill.

--At-Grade fixed guideway station: stations located at street grade along a transit exclusive right-of-way. May include pedestrian overpasses to allow passengers to reach station.

--Underground fixed guideway station:  a concrete structure built below grade, constructed by cut and cover, drill-and-blast, excavated, bored tunnel, or sunken underwater tube.

--Simple at-grade platform station: stations on-street or in street or highway medians. May be low-level platforms (serving low-floor vehicles) or raised platforms (serving high-floor vehicles). Typically includes shelters, canopies, lighting, signage, and/or ticket vending machines.

--Exclusive at-grade separated platform station: stations along the street or in street or highway medians that are separated from mixed traffic. May be low-level platforms (serving low-floor vehicles) or raised platforms (serving high-floor vehicles).

--Additional information on system definition: 
--Legacy heavy rail: This category encompasses some of the oldest transit systems, with roots stretching back to the 19th century. Initially operated by private entities and later transitioned to public management, these systems serve the dense, highly populated regions of the Northeast Corridor and Chicago. They are characterized by older facilities and infrastructure that are integral to the daily commute of millions.

--Post-war subway: Conceived in the 1960s and coming into operation in the 1970s, these systems were developed as a modern alternative to highways, linking suburbs with central cities. Notably, they represent the last major regional subway systems constructed in the United States

--20th Century Systems: a mix of subway and light rail systems that were designed and built in the latter half of the 20th century, ranging from single-line operations to more expansive networks. These systems dot various regions, from the declining populations of "rust belt" cities to the burgeoning metropolises of the West Coast and have experienced various degress of success when it comes to daily use

--Sun belt systems: Located in the rapidly growing southern cities post-World War II, these systems were added between the 1980s and 2000s and located in the Southeast, Southwest, and southern California. They emerged in regions experiencing large population growth and in an era when urban planning heavily favored highways and low-density suburbs.

-- 21st Century Light Rail Systems: Systems that were planned in the 1990s and became operational after 2000 as regional leaders looked to light rail systems as less costly alternative to heavy rail to provide regional rapid transit. These systems often connect cities with their suburbs and are found across diverse regions from the Southeast to the West Coast

--Modern Streetcar Systems: These systems mainly serve smaller cities in the Southeast and Midwest, focusing on downtown revitalization and providing options for tourists and local circulation. They began operation after 2000 and are tailored to areas without the population density or tax base to support larger regional transit systems.

--Bus Rapid Transit (BRT) Systems: These systems are prevalent in smaller cities and are designed as an economical and flexible alternative to rail. They have been operational since 2000 and seek to offer swift transportation options akin to rail services but with the cost-effectiveness and adaptability of road-based transit.

--Commuter Rail Systems: Providing longer-distance, less frequent service, commuter rails connect cities with suburbs and span multiple regions. Often sharing tracks with freight and Amtrak trains, these systems include park-and-ride facilities and have historically served downtown office workers. Post-pandemic, many commuter systems are grappling with greater numbers of people who work from home, fewer commuters, and shifting ridership patterns
