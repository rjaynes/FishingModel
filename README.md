# Fishing Model
A model based on NOAA recreational fishing data

# The data
Here is a link to the data: [link] (https://www.st.nmfs.noaa.gov/recreational-fisheries/data-and-documentation/queries/index)

Data is from the National Oceanographic and Atmospheric Administration(NOAA). The administration conducts ongoing creel surveys throughout the country on an ongoing basis. I focused my data on only the state of Maryland. Catch data comes from those fishing from shore, private boats, charter boats, and party boats. The fishing area is separated into three broad areas: inland, near-shore (within 3 miles of shore), and offshore (over 3 miles out). The fishing season is also separated into 'waves', which are two-month intervals: March/April, May/June, July/Aug, Sept/Oct, and Nov/Dec (January and February are not included). Other columns in the data set include Year, Species group, total number of fish caught, and number of angler trips recorded per survey. I created a 'Catch Per Trip' column that divided total number of fish / number of anlger trips per survey.

<img src="https://user-images.githubusercontent.com/63068643/115759482-49833e00-a36e-11eb-8cd8-fdbfe7ef79d4.JPG" height="200" />

I took the categorical variables (Wave, Mode, Area, and Species Group) and I transformed their entries into dummy variables. Here is the code I used to transform the data:

<img src="https://user-images.githubusercontent.com/63068643/115760166-08d7f480-a36f-11eb-8c98-b44c656c2801.JPG" height="100" />

# Data Exploration
I started by creating simple graphs to see if any trends jumped out. The first thing that became clear was that the majority of angler trips were people either fishing from shore or on a private boat:
<img src="https://user-images.githubusercontent.com/63068643/115761983-f494f700-a370-11eb-998a-a4a3b0473f90.JPG" height="200" />

Also, the vast majority of anler trips were 'inland' as opposed to on the ocean. According to the NOAA website, they categorize Inland as "Inshore bodies of saltwater or brackish water (e.g., bays, estuaries, or sounds). Does not include inland freshwater areas." Maryland borders the Chesapeake Bay, which is the largest estuary in the United States. It stands to reason that the majority of fishing takes place in the bay as opposed to off their much smaller border to the Atlantic Ocean.
<img src="https://user-images.githubusercontent.com/63068643/115761993-f8c11480-a370-11eb-8cd9-2df750cfb929.JPG" height="200" />


Angler trips peaked in the summer, tailing off in the spring and fall. This probably correlates to the local weather and tourism trends more than fish abundance. There was no clear trend from year to year, however.

<img src="https://user-images.githubusercontent.com/63068643/115887431-ece05b80-a41f-11eb-82d3-6fd6ea15b17f.JPG" height="400" /> <img src="https://user-images.githubusercontent.com/63068643/115887438-ef42b580-a41f-11eb-917c-31bfaf9b26f0.JPG" height="300" />

