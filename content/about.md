# About

## Motivation
Philadelphia has a gun violence problem. Homicides have been on the rise since 2013. Last year, 2021, was the deadliest year on record in Philadelphia, with 562 homicides. The city is currently on pace to have nearly as many murders in 2022 as well.

![Homicides Chart](/images/2022_10_31_gun_crime_chart.png)

Community members need solutions , but many city-run initiatives  are frustratingly slow or inadequate . Nearly 80% of the city's anti-violence spending  focuses on long-term violence reduction  without any clear, immediate impact.

## Research
Research shows that greening vacant lots is one of the most impactful, cost-effective interventions available to reduce gun violence in a neighborhood. A recent study found that  greening lots in Philadelphia reduced gun violence by almost 30%  in the surrounding area. 

![Article](/images/main_article_summary.png)

![Greened Lots Examples](/images/transformed_lots.png)

Importantly, community residents know this. They are already following the data and  taking matters into their own hands . This map aims to turn this research into an actionable tool to help community members continue doing what they're already doing.

## Methodology
This map was made by combining Philadelphia crime data with data on vacant lots and "blight" complaints. First, crime data was filtered for only gun crimes (reported as "aggravated assault firearm" and "robbery firearm" by PPD) in the past year, as per the research on which this dashboard is based. These point data were then converted to a  kernel density estimate  layer, which measures the intensity of gun crime at any given point in space.

![Kernel Density Estimate](/images/kde.png)

Next, data from the Department of Licenses and Inspections on vacant lots was cross-referenced with  311 "blight" complaints  to identify vacant lots are currently blighted. Additionally, lots were categorized based on ownership: publicly-owned lots under the  Pennsylvania Horticultural Society's land care program , publicly-owned lots not under PHS land care, and privately owned lots.

Finally, the kernel density estimate layer was extracted to the vacant lots so that each lot was given a gun violence score: a measure of the magnitude of gun violence at and around each particular lot. For ease of use, these scores were scaled from 1 (lowest) to 5 (highest) so that residents can quickly identify which lots in their neighborhoods are associated with the highest rates of gun violence.

![Raster Values to Parcels](/images/values_to_pts.png)

![Parcels by Gun Crime](/images/hot_parcels.png)

## Acknowledgements
Many people helped inform this tool. Pascal Cristofalo, Donna Griffin, Dante Leonard, and Rikeyah Lindsay offered essential perspectives on what features would make this tool most accessible and useful to Philadelphia's communities. Special thanks are due to Drs. Michelle Kondo and Eugenia South, upon whose research this tool is based; to Vicky Tam, who did the spatial analysis for the original research and who taught my GIS class at the Weitzman School of Design; and to Paul Sesink-Clee, who helped me navigate the City's GIS systems.