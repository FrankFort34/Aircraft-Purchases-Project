# Aircraft Purchase Analysis
Author: Frank Fortunati

# Business Understanding
The company is looking to purchase or charter aircraft for the purpose of transporting C-suite and company VIPs efficiently and comfortably. The aircraft may also double as a useful tool for impressing high value company clients. The challenge was to determine which aircraft would be suitable for these goals while also providing a optimal degree of safety.

# Data Understanding
I utilized a data set from the National Transportation Safety Board. The data set was comprised of aviation accident data from 1962 to 2023, and included civil aviation accidents and selected incidents in the US and international waters. The data contained 90,348 rows of accidents spread across 31 columns, such as accident dates, aircraft make and model, injury and aircraft damage severity, and phase of flight when the accident occured. the data set was limited in that key information used for determining overall aircraft safety was not included, such as: distance traveled, average flight time, frequency of inspection, maintenance, and repairs, and accident rate per x number of flights flown. 

Data set: https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses

## Data Preparation
My first goal was to filter out irrelevant or unhelp data from the data set - I did this by filtering out any rows of accidents that were missing information in crucially important fields, such as injury severity, aircraft damage, and aircraft type - this reduced the data from more than 90 thousands rows to 26 thousand. As safety of the aircraft was paramount, I checked the accident rate by number of engines, and concluded all single engine aircraft should be ruled out, as well as any amateur built aircraft. Following this, I included only aircraft that were used for the stated purpose of “Business” or “Executive/Corporate”. Using these filters and parameters, I created two data sets. The first dataset included airplanes, while the second included on helicopters.

# Exploratory Data Analysis
With both the airplane and helicopter data sets, I broke down the accidents by degrees of severity (Destroyed, Substantial, and Minor) and sorted them by manufacturers. From there, I analyzed specific models with minor accidents. For the airplane data set, I took a closer look at models from Cessna, Piper, Raytheon, Beech, and Bombardier, which I then compared. I focused then on the models with the lowest accident rate: the Cessna 560, the Bombardier BD100 1A10, and the Piper PA-34-24OT. I performed a similar analysis for the helicopter data set and determined a suitable recommendation, the Sikorsky S-76A




![Aircraft Accident Comparison](https://github.com/user-attachments/assets/8aacf187-db31-4b02-b336-da62c9e4df36)


 
# Conclusion
After examining the aviation accident data set, as well as considering the limitations of this dataset, as described below, I would recommend the company consider small or medium sized business jets for purchase or charter. I also recommend the company examine executive business helicopters as an alternative to jets.

## Limitations
The data set used included aviation accidents only, requiring further research into aircraft costs. 
The primary limitation is that a complete safety evaluation cannot be completed with the data, as the data set includes only aviation accidents and does not include other relevant aircraft information, such as: average fuel cost, average travel distance, maintenance costs, inspection and repair frequency, etc. 

## Recommendations
I recommend the company consider the Cessna 560 and the Bombardier BD100 1A10 aircraft for transporting C-Suite and VIPs in a jet. Additionally, I'd also recommend the Sikorsky S-76B helicopter as an alternative to the jets.

## Next Steps
Further analysis that includes model specific flight data and safety would be beneficial. Research should address the areas of limitation stated above, including average travel distances, frequency of repair and maintenace, etc. 

## For More Information
Please see the full analysis in the Jupyter Notebook, linked below, or review this presentation: [Aircraft Purchase Analysis.pdf] (https://github.com/user-attachments/files/19539026/Aircraft.Purchase.Analysis.pdf)
For additional information, contact Frank Fortunati at fortunatifrank@gmail.com

https://github.com/FrankFort34/Aircraft-Purchases-Project/commit/5ae0815bccfcea1297875b6ca8a049975b9de576



