# Red Flag!: Spotting Potential Illegal Fishing Activity Using AIS Outage Data

Data storytelling project — Master of Data Science, University of Pittsburgh.
Analysis of 55,368 AIS disabling events published by Global Fishing Watch (2017–2019).

**[Read the full data story →](https://cmckean2018.github.io/Spotting-Potential-Illegal-Fishing-Activity-Using-AIS-Outage-Data/McKean_Data_Story.html)**

## Figures

### 1. Visualizing 'Hot Spots'
Across every ocean, AIS disabling clusters into a small number of distinct areas. This heat map shows that there are large numbers of AIS outage events taking place off the coast of South America, Africa, Japan, and Papua New Guinea. AIS outage 'hot spots' are at a higher risk of illegal fishing practices.

![Global heatmap of AIS disabling events](figures/figure1_map_preview.png)
**[Open the interactive map →](https://cmckean2018.github.io/Spotting-Potential-Illegal-Fishing-Activity-Using-AIS-Outage-Data/figures/figure1_map.html)**


### 2. Vessels go dark near EEZ boundaries
9,905 AIS disabling events begin in the 20 nautical miles just outside the EEZ. 69% of these events are on the Patagonian Shelf. Fragmented jurisdiction and limited enforcement capacity on the high seas make it easier for boats to turn off tracking and overfish without being caught. Vessels that are guilty of illegal fishing will often turn off AIS when approaching the outer limit of an EEZ. This allows foreign or otherwise unauthorized vessels to sneak in without permission.

![Distance from shore](figures/figure2_distance_from_shore.png)

### 3. AIS disabling events align with the seasonality of fisheries
Squid jiggers are present in mass only during squid season (Jan - Apr) and then disappear during the winter. However, trawlers that are fishing the same waters in the same months, under the same satellites, show no comparable seasonality in AIS outages. If thin satellite coverage or bad weather over the South Atlantic were darkening transponders, it would darken trawlers and jiggers alike. Instead, the squid jigger fleet's disabling follows its target species' calendar, which points to suspicious behavior rather than failing infrastructure.

![Patagonian seasonality by gear](figures/figure3_patagonia_seasonality_by_gear.png)

## An important caveat

Disabling AIS is not proof of illegal fishing. Transponders fail, satellite coverage has gaps, and vessels sometimes go dark for legitimate reasons including piracy avoidance and protecting productive fishing locations. These figures provide recommendations for where increased surveillance would be the most productive, not where illegal activity has been established.

## Data

Global Fishing Watch AIS disabling events, 2017–2019: 55,368 events from 5,269 commercial fishing vessels. Gaps shorter than 12 hours and those beginning within roughly 50 nautical miles of shore are excluded by the data provider. The source CSV is not included here, you can download it from Global Fishing Watch.

## Contents

- `McKean_Data_Story.ipynb` — full analysis
- `McKean_Data_Story.html` — rendered version of the notebook
- `figures/` — exported figures and the interactive map

## Tools

Python · pandas · NumPy · matplotlib · folium
