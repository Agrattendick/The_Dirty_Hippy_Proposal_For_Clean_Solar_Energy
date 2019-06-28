# The Dirty Hippy Proposal for Clean Solar Energy

## Description
This project uses Google's [Project Sunroof](https://www.google.com/get/sunroof) data to examine the costs and benefits solar panel installation on individual homes. Right now roofs keep us dry and protect us from the elements. Can they do more? (The null hypothisis is no. Current Panels are too expensive and not efficient enough to provide a benefit.)

![sun](Images/sun.jpg)

## Possible Complications
Google provides some wonderful data, and this report relies heavily on their datasets. Their outlook is bright, however in some ways their datasets are incomplete. For example their sunny disposition shines through in their yearly_sunlight_kwh_kw_threshold_avg computation. Google assumes a loss of 25% of sunlight over a year. Using the Open Weather Map API, this information is replaced with a more accurate figure by area. Southern California may lose less than 25% while New Jersey weather might consume more. Most solar panels still work with cloud cover, they are just much less efficient. On clouldy days they produce 25% of normal, and on very cloudly days only 10% of normal.

Another issue is existing power plants. More importantly the type of existing plants. If the main power source for a house is a coal plant, solar panels on a personal residence might provide a benefit. If the power plant uses nuclear or renewable sources for energy there is no carbon offset. This project will look at the amount of power produced by each energy source on a state level, and factor that into the possible benefits for home based solar panels.

## Datasets
* Google Project Sunroof CSV Files:
    * Projected Power generated by roofs in searched areas
    * Projected CO2 offset.
    * [Google Project Sunroof](https://www.google.com/get/sunroof)

* Open Weather Map API:
    * Cloudiness of searched area.
    * [OpenWeatherMap](https://openweathermap.org/)

* Power Production Excel:
    * Ammount of electricity from fossil fuels, nuclear power, and renewable energy by state.
    * [eGRID Summary Tables](https://www.epa.gov/energy/egrid-summary-tables)  
    * Ammount of CO2 produced by various power sources.
    * [How much carbon dioxide is produced when different fuels are burned?](https://www.eia.gov/tools/faqs/faq.php?id=73&t=11)

* State Information  
    * State Landmass.  
    * [United States Summary: 2010, Population and Housing Unit Counts, 2010 Cenus of Population and Housing via Wikipedia](https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_area)  
    * State Populations  
    * [Table 1. Annual Estimates of the Resident Population for the United States, Regions, States, and Puerto Rico: April 1, 2010 to July 1, 2018 (NST-EST2018-01) via Wikipedia](https://en.wikipedia.org/wiki/List_of_states_and_territories_of_the_United_States_by_population)
    * State Power Consumption
    * Need to find information on how much power each state uses.

## 3 - 5 Initial Research Questions:
* Are personal solar panels a benefit for homeowners?
    * what is the financial benefit of solar power v. cost of installation?

* Does living in a high density or low density housing make a difference?

* How does a community benefit from personal solar panels for homeowners?
    * How much carbon offset is provided by solar cells?
    * How much power is currently provided by fossil fuels?

* How big is the carbon offset?
    * Is the carbon offset reason enough to switch over to solar power? Should the government subsidize insalation for that reason?

## Progress
The bar graphs showing carbon offset came out great.

Actually plotting the scatter plots of carbon offset by landmass raised new questions. Landmass isn't as great as originally thought. There's variation in population density. That was considered, and more scatter plots were to show this adjucting for pop density. Current thoughts lay around the roof counts in the Project Sunroof dataset.  
  
The scatter plot for adjusted carbon offset by state population looks fine. Want to work on a residual plot, and added a power consumption by state population scatter plot to the to-do list.

The work currently revolves much more around carbon offset than financial benefits. Perhaps financial benefits isn't all that important, and if there isn't much of a benefit Google's project solar should look to states to subsidize the cost in an effort to become more carbon friendly? It'd also help states become carbon neutral for international agreements. (It's something to look into, but also project creep?)

# GitHub Link
[GitHub](https://github.com/Agrattendick/The_Dirty_Hippy_Proposal_For_Clean_Solar_Energy)