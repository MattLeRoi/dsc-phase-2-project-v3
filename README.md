# Film Analysis

**Author**: [Matt LeRoi](mailto:mcleroi@gmail.com) 

# Business Understanding

The goal of this project is to advise ACME Co, who are new to the film industry, on how they can maximize their odds of making financially sucessful films. 

# Data Understanding

This project uses two data sources: [financial data](./data/tn.movie_budgets.csv.gz) from The-Numbers.com and [detailed film data](./data/im.db) from IMDB.com. The financial data includes the cost of making each film and the domestic and worldwide grosses. The detailed film data includes things like the runtime, applicable genres, and user ratings. 

## Data Preparation

The two files are trimmed of unecessary information and formatted in a consistent manner to be merged later. This includes converting strings to numbers and dates, and renaming columns to match between the two data sources.

# Exploratory Data Analysis

The profit and return on investment (ROI) percentage are calculated for each film and the two data sources are merged. Models are created for each output - profit and ROI - showing the statistically significant factors and the effect of each. 

# Conclusion

The rates of aircraft issues varied greatly from aircraft to aircraft. Within the top 10 most common single and dual engine aircraft, the rates varied from 5 occurrances per 1000 registered aircraft to 25.  

![Tables.png](./Images/Tables.png)

There were no significantly noted differences in accident rates between single and dual engine aircraft. The number of people affected was different, however, due to the generally larger seating capacity of dual engine planes. 

![Stacked.png](./Images/Stacked.png)

![Bar_chart.png](./Images/Bar_chart.png)

## Limitations

The available data only provide the number of incidents, severity of injuries, and number of aircraft registered. Many other factors pertaining to the incidents could provide more detail about which incidents were related to the aircraft and which were pilot error, weather related, or otherwise independent of the aircraft. Also, the registration data seems a reasonable factor for normalizing incident counts, but number of hours or miles flown would be a more accurate normalization factor. 

## Recommendations

The following aircraft are recommended for further study:

Single engine aircraft:
- CIRRUS DESIGN SR22T
- PIPER PA-28-180
- PIPER PA-28-181

Dual engine aircraft:
- BD-100-1A10
- LEARJET INC 45
- BEECH 95-B55 (T42A)
- PIPER PA-23-250

## Next Steps

The recommended aircraft should be further analyzed for other factors, including:
- Acquisition cost
- Maintenance cost
- Fuel cost
- Staffing requirements
- Lifetime of aircraft / performance over time
- Availability of pilots and crew
- Seating capacity

## For More Information

See the full analysis in the [Jupyter Notebook](./Aircraft_safety.ipynb), review this [presentation](./Slides.pdf), or peruse this [dashboard](https://public.tableau.com/app/profile/matthew.leroi/viz/Aircraft_safety/Dashboard?publish=yes).

For additional info, contact Matt LeRoi at [mcleroi@gmail.com](mailto:mcleroi@gmail.com)

```
├── data
├── images
├── README.md
├── Slides.pdf
└── Aircraft_safety.ipynb
```
