# 94% of Brazil's donkey slaughter happened in one facility in 2025

## What I aimed to accomplish

My goal was to use GeoJSON and Datawrapper to build the map I envisioned,
then refine it in Illustrator — though that last step proved too difficult
and I eventually set it aside. I also wanted to analyze data obtained from
Brazil's Ministry of Agriculture and Livestock (MAPA) to verify whether the
documents aligned with what Brazilian researchers claim: that the
slaughterhouse in Amargosa is the country's largest exporter of donkeys to China.

## Short description of my findings

Official records from Brazil's Ministry of Agriculture and Livestock (MAPA)
show that donkey slaughter in Brazil is effectively a one-state operation, what researchers in the field had already been saying.
In 2025, four federally inspected slaughterhouses processed a combined total
of 21,970 donkeys — and a single facility, Nordeste Pecuária in Amargosa,
Bahia, was responsible for nearly 94% of that total, slaughtering 20,594
animals at an average of 1,716 per month.


## Summary of the data collection process

The data was obtained through a formal information request made by a federal
congressman to MAPA. The dataset covers donkey slaughter records
across federally inspected facilities in Brazil from 2021 through 2025.
Slaughterhouse addresses were also provided by MAPA and cross-checked against
Brazil's CNPJ registry (Federal Revenue Service).

- [MAPA - Adresses of the slaughter houses](https://drive.google.com/file/d/1hgv0q9O1M15ls4hfVkf5PmSddF5MiT84/view?usp=sharing)
- [MAPA - sDonkey slaughter from 2021 through 2025](https://docs.google.com/spreadsheets/d/1TmJY0HdhNaQFhXvHI2DforLa_noQF60n/edit?usp=sharing)
- [Congressional request (PDF)](https://drive.google.com/file/d/1QNeP4gE9_y6IDMo4P4UZMRuD-2WnEBD4/view?usp=sharing)

## Overview of the data analysis process

The data was analyzed using Python and pandas in a Jupyter notebook. The
main steps were:

- Loaded the full dataset (4,778 rows) and filtered for 2025 records
- Grouped slaughter totals by facility and municipality
- Calculated the monthly average per facility (`Qtd Abate / 12`)
- Sorted results to identify the largest slaughterhouse by volume

The analysis confirmed that Nordeste Pecuária (Amargosa, BA) far exceeded
all other facilities, with 20,594 animals slaughtered.

- [Jupyter notebook](analysis-MAPA.ipynb)

## What new skills and approaches I developed

- Working with GeoJSON files to create geographic visualizations
- Building and customizing maps in Datawrapper
- Analyzing CSV data using pandas

## Things I tried to do or wanted to do but did not have the skills/time

- I was not abble to put annotations on my map with Illustrator, it was too difficult for me 