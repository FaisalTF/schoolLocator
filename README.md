## Washington Public School Locator
This project showcases public schools around the state of Washington. A list of all current public schools in Washington State for the 2021-2022 school year as listed on the OSPI School Directory is presented to the user, who may explore the directory, the map, and choose a certian school for the map to zoom into and showcase information about.

#### This project was built with four main utilities in mind:

1- To serve as a pltform visualizing broad geographical trends in the distribution of schools aorund the state of Washigton. This could help identify disparities in educational opportunities across different geographical and socioeconomical factors.

2- To visualize schools in proximity to a specific address or monument; this could help identify the strength of a single address through the educational opportunities in proximity. This could be helpful, for example, in comparing resedential addresses and assessing property decisions.

3- To visualize schools relative to each other, providing the ability to compare different schools and clustering trends.

4- To serve as a school directory. The comprehensive list of schools is listed along with addresses, and can serve for those looking to browse or locate a school. The information present can also easily be expanded to show more information that is already present within the data.


The platform is at the following link: https://faisaltf.github.io/schoolLocator/index.html


Below are snippets from the app:



<img width="1440" alt="Screen Shot 2021-12-12 at 10 58 48 PM" src="https://user-images.githubusercontent.com/74882570/145786267-d245d271-a4fd-4a25-bb39-7db91909a051.png">


 

<img width="1440" alt="Screen Shot 2021-12-12 at 10 59 41 PM" src="https://user-images.githubusercontent.com/74882570/145786283-001e8fc8-99ed-40c5-bff9-d34edf09ed84.png">



### The web application currently includes the following features:
An interactive map – the map displays school locations around Washington and can be explored through zooming in/out or moving around the map.

A directory list that showcases all the available schools, a short description with addresses. Each school item may be clicked for the map to zoom on to the specific item. Additionally, a popup on the map shows up with the school information.

Geocoding – A search bar is present at the corner for users to look up addresses or locations. These locations do not have to be existing schools or data points, as the search query is geocoded using mapbox’s geocoder. A resulting list from places around Washington shows up, where each item may also be seleceted and zoomed into on the map.


### Potential Features to be Added:
Auto sorting – some of which is already implemented but not functional yet; this would update the list of schools every time an item (school or geocoded location) is selected based on proximity. 

Filtering – The data source from the Office of Support of Public Instruction (OSPI) includes much more information about each school. This may allow the web app to expand a filtering tab where schools can be hidden/shown based on different attributes. Filtering may also be added through colors to help distinguish further trends around schools in Washington.

### Data Sources:
The school data comes from the Washington Geospatial Open Data Portal, where it was posted by the Office of Support of Public Instruction (OSPI). As previously mentioned, this includes information on all public schools in Washington State for the 2021-2022 school year according to OSPI.

Here is the link to the source:
https://geo.wa.gov/datasets/k12wa::washington-state-public-schools/explore?location=47.290385%2C-120.802250%2C7.52.

### Technical Frameworks Used:
The project directly utilizes the open-source packages listed below. Additionally, GeoJson.io and QGis were both used in exploration phases before the building of the web app. The geocoder module was also implemented, allowing the search feature on the app to display geocoded locations from Washington.

Mapbox GL JS: a a client-side JavaScript library for building web maps and web applications with Mapbox's modern mapping technology.  Mapbox was used for the interactive map layout and visualizing the data.

Turf.js: a modular geospatial analysis package. Though the functionality is not currently working on the live page, turf js is imported to try to re-sort the schools list by distance.

### Acknowledgements:
Most of the tool methods taught in this project were taught in in the course Geography 495: Web & Mobile GIS at the University of Washington – Seattle, taught by Professor Bo Zhao and Assisted by Steven Bao. This project also took technical inspiration from different tutorials posted by the mapbox documentation.
