# forest-fire

## Data
The data focus is on the ISI which correlates to the velocity of fire spread. It´s related to the Forest Fire Weather Index which was a system developed in canada for rating the threat of forest fires , and has subsequently been proven to fit in the Mediterrenian forests (Cortez and Morias "A Data Mining Approach to Predict Forest Fires using Meteorological Data")

## Business Questions
*The major concern is the role of seasons in ISI rating. 
The common questions include, what season do most fires take place?
As fire prevention also might require the presence of active workforce for early detection, the absence of a workforce due to weekends was also evaluated. As we don´t have full control of the data details, it was hard to factor in public holidays and the normal work schedule of forest managers.

## Findings
Fire occurence by season: The analysed chart (see in image file titled: Fire recording by seasn) shows much of the fire incidents recorded were in summer, followed by autumn, spring and winter respectively.
The ISI ratings also corresponded to the chart with higher ISI average in Summer recorded at 10.89, autumn at 8.42, spring at 6.79 , with winter at a mere 3.26 ISI rating 8(see barchart ISI by season)
ISI rating average were tested to see if there was a significant difference between as´verages recorded in weekend vs weekday, using a one way ANOVA: With a p-value 0.46 which was greater than the α (0.05), we conclude there is no significant difference betweenn the ISI RATING ON THE DAY OF THE WEEK:

## Modelling
A model was fitted using the decison tree (see image: model). Fewatures used were 
Cordinates 'X' and 'Y' 
Fine Fuel Moisture Code (FFMC) which represents the mositure content surface litter,
Duff Moisture Content (DMC) and the Drought Code (DC)
Environmental factors like Season, Temperature (temp), relative humidity (RH), wind, rain. And other factors like Day, and total area affeted 
The model performed well on the data train set but was poor on the test set and could be overfitting.
As modeling was not the main feature of this project subsequent project will be carried to find the best fitting model.
