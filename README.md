Electric Vehicle Next Charge Location Prediction

This repository contains the following folders: 

Code
	
a) BATCH_PADDING.ipynb
This file contains functions to prepare data for modelling, all code is fully commented. Functions include creating batches, padding batches, and analysis of data.  

b) MODELLING.ipynb 
This file contains all scripts required to prepare and model data using both BiLSTM and CNN fastai models, all code is fully commented.

c) BATTERY_MASK.ipynb 
This file is used to mask charge cycles to represent different battery charge levels to model data representing a variety of battery charge ranges.


Docs

a) Chicago City Map.afphoto
This file is a map for Chicago city which has 77 community areas, these community areas are taxi passenger pickup and drop off locations as well as possible EV next charge location prediction areas.

b) Chicago-Charge-Stations.xlsx
This file is a list of service stations and their addresses including the community area ID, we assume these service stations will be charge stations in the future.


Data

This folder contains all datasets including: 

a) 12 months of EV taxi spatio-temporal datasets every month divided into 3 CSV files, each CSV file has a header including all feature titles.

b) A CSV file which is a data_dictionary.csv explaining features in our EV monthly CSV files.

c) EV_Sales.xlsx this file contains logistics for the 9 EVs including battery capacity kWh, range in Kilometres (km), energy consumption Wh/km, sales 2019, and total sales within the USA.

d) A file called period.xlsx this file contains 7 periods of a 24 hour day including start and end time for these periods.

e) ChargeStations.xlsx this file contains 77 community areas and the number of petrol/service stations that these communities have, we assume these service stations will be charge stations in the future.

f) location_boundary.xlsx this file contains community areas ranging from 1 to 77 in the first column, followed by community areas that share a common border with the community area in the first column.
 
