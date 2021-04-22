# Fishing Model
A model based on NOAA recreational fishing data

# The data
Here is a link to the data: [link] (https://www.st.nmfs.noaa.gov/recreational-fisheries/data-and-documentation/queries/index)

Data is from the National Oceanographic and Atmospheric Administration(NOAA). The administration conducts ongoing creel surveys throughout the country on an ongoing basis. I focused my data on only the state of Maryland. Catch data comes from those fishing from shore, private boats, charter boats, and party boats. The fishing area is separated into three broad areas: inland, near-shore (within 3 miles of shore), and offshore (over 3 miles out). The fishing season is also separated into 'waves', which are two-month intervals: March/April, May/June, July/Aug, Sept/Oct, and Nov/Dec (January and February are not included). Other columns in the data set include Year, Species group, total number of fish caught, and number of angler trips recorded per survey. I created a 'Catch Per Trip' column that divided total number of fish / number of anlger trips per survey.

![dataset](https://user-images.githubusercontent.com/63068643/115759482-49833e00-a36e-11eb-8cd8-fdbfe7ef79d4.JPG)

I took the categorical variables (Wave, Mode, Area, and Species Group) and I transformed their entries into dummy variables. Here is the code I used to transform the data:
