# Green-AI - Deforestation tracking with AI 

 

 

 

1-Minute Preliminary Presentation Script for "AI-Powered Deforestation Tracking" 

Our team has chosen "AI-Powered Deforestation Tracking" as the topic for our project, which falls under the "Environment protectionl" category mentioned in the project guide . 

Deforestation is a critical environmental issue—losing forests disrupts ecosystems, worsens climate change, and threatens biodiversity. Traditional tracking methods (like manual surveys) are slow and limited in coverage, but AI can solve this by analyzing satellite or aerial images to detect deforestation areas quickly and accurately. 

So far, we’ve started reviewing existing AI applications in this field, such as using deep learning for land cover classification to spot deforestation hotspots. Next, we’ll search for 2 related papers via Arxiv, check if their data (like satellite image datasets) is open-source or publicly available, and confirm the access steps as required . 

We believe this topic matters because AI-driven tracking can help governments and NGOs take timely action to protect forests. That’s our preliminary plan—thank you! 

 

STATE OF ART 

1)Why deforestation is a problem  

 

-Environmental cause 

 

Environmental issues are among the most pressing challenges of our time. Human activities, combined with natural processes, have triggered large-scale transformations in the Earth’s ecosystems. These changes affect biodiversity, climate stability, and human livelihoods. The main causes of environmental degradation can be grouped into several key categories: 

    Deforestation and Land Use Change 
    Forests are being cleared at alarming rates for agriculture, urbanization, and mining. This leads to habitat loss, increased greenhouse gas emissions, soil erosion, and disruption of the water cycle. In tropical regions, deforestation is also linked to illegal logging and expansion of cattle ranching. The loss of tree cover reduces the planet’s capacity to absorb carbon dioxide, directly accelerating global warming. 

    Climate Change 
    The combustion of fossil fuels for energy, transportation, and industry releases massive amounts of CO₂ and other greenhouse gases. This alters global temperature patterns, causing extreme weather events such as heatwaves, floods, and droughts. Melting glaciers, rising sea levels, and shifts in ecosystems are some of the long-term consequences. 

    Air and Water Pollution 
    Industrial emissions, vehicle exhaust, and agricultural runoff contaminate both air and water sources. Air pollution contributes to respiratory diseases, while polluted rivers and oceans threaten aquatic life and food security. Plastic pollution, in particular, has become a global crisis, affecting marine ecosystems and entering the food chain. 

    Soil Degradation and Desertification 
    Unsustainable agricultural practices—such as overgrazing, deforestation, and excessive use of fertilizers—lead to soil exhaustion and loss of fertility. Over time, this can result in desertification, especially in arid and semi-arid regions, reducing the availability of arable land and threatening food production. 

    Loss of Biodiversity 
    Species extinction rates are accelerating due to habitat destruction, pollution, and climate change. The loss of biodiversity weakens ecosystem resilience and reduces essential services like pollination, water purification, and carbon storage. 

    Urbanization and Waste Generation 
    Rapid urban growth increases demand for energy, transportation, and infrastructure, leading to higher emissions and waste production. Inadequate waste management causes land and water contamination, while expanding cities encroach on natural habitats. 

 

-Why is it difficult to observe 

 

Why Deforestation Is Difficult to Observe 

Monitoring deforestation accurately and in real time is much harder than it may seem. Even with modern satellite technology, several factors make the process challenging: 

    Cloud Cover and Atmospheric Conditions 
    In tropical regions like the Amazon or Central Africa, clouds are present almost all year. Optical satellites such as Landsat or Sentinel-2 cannot capture clear images through clouds, meaning large areas are often invisible for weeks or even months. This causes delays and gaps in monitoring. 

    Data Availability and Temporal Resolution 
    Even when satellites revisit the same area frequently, not all images are usable because of cloud shadows, haze, or poor lighting conditions. Detecting subtle or gradual deforestation (like selective logging) requires long, clean time series, which are often incomplete. 

    Spectral Similarity and Noise 
    The difference between healthy forest, degraded forest, or cleared land can be small in spectral terms (the colors and intensities detected by sensors). Noise from sensors, variations in soil moisture, or seasonal vegetation changes can easily mask true deforestation signals. 

    Mixed Land Cover and Partial Disturbances 
    Deforestation doesn’t always happen as a clean cut of large forest blocks. It often starts with scattered tree removal, small fires, or road building. These subtle changes are hard to detect with coarse satellite resolutions or simple classification models. 

    Radar Data Complexity 
    Radar sensors (like Sentinel-1) can see through clouds, but their data is noisy and harder to interpret. Backscattering values depend on surface roughness and moisture, not just on vegetation presence, which complicates deforestation detection. 

    Validation and Ground Truth 
    Satellite-based detections must be validated with on-the-ground observations or high-resolution imagery. In remote or dangerous areas, this is difficult, expensive, and sometimes impossible, leading to uncertainties in accuracy estimates. 

 

2) Existing methods to track deforestation 

 

 

3) Solutions to the problem : 

-	Stop using paper 

-	Stop eating woods 

-	Start hugging tree roots 

 

 

4) Research limitations 

# Data From Our World in data (https://ourworldindata.org/deforestation)

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Annual deforestation rate
The conversion of forest to other land use or the long-term reduction of the tree canopy cover below the
minimum 10 percent threshold. Deforestation implies the long-term or permanent loss of forest cover and implies transformation into another land use. Such a loss can only be caused and maintained by a continued human-induced or natural perturbation.
Unit conversion factor: 1000  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
UN Food and Agriculture Organization (FAO). Forest Resources Assessment. – processed by Our World in Data

#### Full citation
UN Food and Agriculture Organization (FAO). Forest Resources Assessment. – processed by Our World in Data. “Annual deforestation rate” [dataset]. UN Food and Agriculture Organization (FAO). Forest Resources Assessment. [original data].
Source: UN Food and Agriculture Organization (FAO). Forest Resources Assessment. – processed by Our World In Data

### Additional information about this data
Raw data for forest area, deforestation, afforestation and expansion is sourced from the UN FAO Forest Resources Assessment.

Our World in Data have calculated several metrics based on this raw data including:
– Net change in forest area (afforestation minus deforestation)
– Net conversion rate (net change as a percentage of forest area)
– Each country's share of global forest area, deforestation, afforestation, and net change in forests
– Each country's share of regional forest area, deforestation, afforestation, and net change in forests

The UN FAO publish forest area and forest change data as the annual average on 10- or 5-year timescales. Therefore the following year allocation applies:
– 1990: the annual average over the period from 1990 to 2000.
– 2000: the annual average over the period from 2000 to 2010.
– 2010: the annual average over the period from 2010 to 2015.
– 2015: the annual average over the period from 2015 to 2020.

Data on forest cover by country pre-1990 is sourced from a variety sources which are documented here: https://docs.google.com/spreadsheets/d/1nYpao4e8Ai-P86jIUZ3r7X6-5MjZ7ZbG7TJQSO729Bg/edit?usp=sharing


    
