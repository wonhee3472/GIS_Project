# Purpose
After Dana (my wife) is finished with her grad school in about 1.5 years later from now, we are planning on moving back to one of the suburbs in Chicago. But we want to go somewhere safe where there isn't that much crime activity in the area. This data exploration and visualization will help us to decide which area we'd like to choose as our next home in Chicago. 

# Approach
I accessed the data extracted from the [Chicago Police Department](https://data.cityofchicago.org/Public-Safety/Crimes-One-year-prior-to-present/x2n5-8w5q) by using the Sodapy library and Socrata Open Data API. With the extracted and modified dataset, I mapped the coordinates of arrest made in Chicago in Jan 2022 by using the Kepler library.

# Result
To see the steps I took to do analysis, click here [Chicago_Crime](https://github.com/wonhee3472/GIS_Project/blob/main/Chicago%20Crime.ipynb).
To see the result of the analysis, clicking the raw version of [chicago_arrests.html](https://github.com/wonhee3472/GIS_Project/blob/main/chicago_arrests.html) won't work. You probably have to clone this repostitory and open [this file](https://github.com/wonhee3472/GIS_Project/blob/main/Chicago%20Crime.ipynb) with jupyter notebook in a new conda environment where you have `geopandas`, `sodapy`, and `keplergl` installed. But since it can be a little difficult to know how to use features included in `kepler`, I attached the screenshot [here](https://github.com/wonhee3472/GIS_Project/blob/main/snapshot_crime_chicago.png) so that people can see the outcome I've acquired at the end.

# Reflection
The website [Chicago Police Department](https://data.cityofchicago.org/Public-Safety/Crimes-One-year-prior-to-present/x2n5-8w5q) gives you the option to see their version of data visualization (it can be found if you scroll all the way down). It has a lot of embedded features that enable the users to interact with the map but in my opinion, it's a little difficult to get the whole picture by just simply glancing at it and I feel like it's hard to use the filter feature. I think the `kepler` library has a very powerful tool where you can make the map 3-D and it's relatively easier to mess around with it.

There's one aspect I didn't get insights from this dataset. If you manage to get the environment to work to see the work I did, you'll see that the data only applies to Chicago, not the suburubs of Chicago which is where I want information for. In other words, unless I'm trying to get a house in Chicago (very very unlikely), this exploration of data may not help me make decisions unfortunately. :(
