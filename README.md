**Electric-Vehicle-Next-Charge-Location-Prediction**

**This repo contains**


	README.md contains a list of folders and their contents. Steps to follow using the jupyter code.

	1) First use the BATCH_PADDING.ipynb, this file has all the scripts required to prepare data for modelling, all scripts are fully commented.

	2) Second the MODELLING.ipynb, this file has all the scripts required to prepare and model data insluding for BiLSTM and CNN models, all scripts are fully commented.

	3) The BATTERY_MASK.ipynb files is used to mask charge cycles to represent different battery charge levels to model for
	   a variety of battery charge ranges.



	**And the following 3 folders:**
	
	**1) docs**

	This folder contains a Chicago city map with 77 community areas, these community areas are used in this use case for EV next charge location predicition problem area.

	
	**2) data**

	This folder contains all datasets including: 

	- 12 months of ev taxi spatio-temporal datasets, each month of the year seperated into individual csv files.
	
	- data_dictionary.csv explaining features in our ev monthly csv files.

	- EV_Sales.xlsx this file contains logistics for the 9 EVs including battery capacity kWh, range in km, energy 
	  consumption Wh/km, sales 2019, and total sales within the USA.
	
	- period.xlsx this file contains 7 periods of a 24 hour day including start and end time for these periods.

	- ChargeStations.xlsx this file contains 77 community areas and the amount of petrol stations which we assume will be 
	  charge stations in the future.

	- location_boundary.xlsx this file contains community areas from 1 to 77 in the first column, followed by community 
	  areas that share a common border with the community area in the first column.


	**3) code**

	- BATCH_PADDING.ipynb this jupyter notebook file contains scripts to batch, pad, and analyse data to get it ready for 
	  modelling.  

	- BATTERY_MASK.ipynb this jupyter notebook file contains scripts to mask each batch so they can be used in modelling 
	  for a range of battery charge levels. 

	- MODELLING.ipynb this jupyter notebook file contains scripts to prepare and model using both Bidirectional LSTM 
	  (BiLSTM), and Convolutional neural network (CNN) being a fastai xresnet18 both pretrained and non-pretrained. 
 
