# Forest transition phase - Data package

This data package contains the data that powers the chart ["Forest transition phase"](https://ourworldindata.org/grapher/forest-transition-phase?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on December 03, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Forest Transition Phase


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Forest Transition Phase (Pendrill et al. 2019) – processed by Our World in Data

#### Full citation
Forest Transition Phase (Pendrill et al. 2019) – processed by Our World in Data. “Forest Transition Phase” [dataset]. Forest Transition Phase (Pendrill et al. 2019) [original data].
Source: Forest Transition Phase (Pendrill et al. 2019) – processed by Our World In Data

### Additional information about this data
The study categorized countries into four categories based on their stage in the forest transition.

As, detailed, they follow a similar framework to Hosonuma et al. (2012).

"Countries exhibiting low deforestation rates are classified as pre- or post-transition depending on whether forest cover is high or low (or if net reforestation is occurring); countries with high deforestation rates are classified as early-transition if gross deforestation is increasing and remaining forest cover is not too low, and late-transition otherwise. We decided to use a slightly lower threshold than Hosonuma et al (2012). We also manually adjusted the classification for a few post-transition countries that were not classified as such and excluded countries with less than 5% forest cover."

Hosonuma describe the Forest Transition Model as:
"The four FT phases are pre-transition, early transition, late transition and post-transition, which generally represent a time sequence of national development. Pre-transition countries have high forest cover and low deforestation rates. In early-transition countries, forest cover is lost at an increasingly rapid rate. Late-transition countries with a rather small fraction of remaining forests exhibit a slowing of the deforestation rate and eventually come into the post-transition phase, where the forest area change rate becomes positive and forest cover increases through reforestation. The FT model reflects a broad-scale typology of tropical developing countries, applicable as a proxy for analyzing the temporal variability of drivers of deforestation and forest degradation."

Additional references:
Hosonuma, N., Herold, M., De Sy, V., De Fries, R. S., Brockhaus, M., Verchot, L., ... & Romijn, E. (2012). An assessment of deforestation and forest degradation drivers in developing countries. Environmental Research Letters, 7(4), 044009.


    