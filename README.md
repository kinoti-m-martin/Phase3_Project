# Phase3_project
## 1. Project Overview
This project inlves the analysis of the `Traffic Crashes in Chicago`, and obtaining insights on the main contributors to these incidences, as directed by the government.

## 2. Problem Statement
The city of Chicago is experiencing an increased number of traffic accidents on its roads, where we are tasked with investigating the causes, and come up effective solutions.

## 3. The Data
The data used in this project is `Traffic Crashes` dataset, that is present in this repository. This data was collected in Chicago, regarding the trends of their traffic accidents. The data contains several data classes, which include:
* crash_record_id: This is the unique identifier of the data,
* rd_no: The specific road
* crash_date: The date of the crash
* posted_speed_limit: the speed at time of the accident.
* traffic_control_device: device controlling the traffic
* device_condition: the condition of the traffic control device
* weather_condition:weather condition at time of the accident,
* lighting_condition: road lighting condition
* trafficway_type: type of traffic involved
* lane_cnt: number of lanes on the road
* alignment: the alighnment of the road at crash spot
* roadway_surface_cond: the general condition of the road
* road_defect: the defect present on the road surface
* crash_type: the type of crush involved- either there was injuries or not
* intersection_related_i: whether the accident occured at an intersection 
* not_right_of_way_i: no right of way in place
* hit_and_run_i: hit and run incident
* damage: the general degree of damages observed
* prim_contributory_cause: the main cause of the accident
* dooring_i: vehicle door related accidents
* work_zone_i: construction work zone
* work_zone_type: construction type
* workers_present_i: number of workers present on site
* most_severe_injury, injuries_total, injuries_fatal, injuries_incapacitating, injuries_non_incapacitating,injuries_reported_not_evident, injuries_no_indication
* crash_hour: time of the crash
* crash_day_of_week: the week of the crash
* crash_month: the month of the crash
* latitude, longitude, location: location where the accident took place

## 4. Data Analysis
Data analysis involved the exploration of the categorical and numerical DataFrames, which was done immediately after data cleaning. The relationship between the target column(damage), and the independent variables was also explored.

## 5. Preprocessing
Data preprocessing was done before modelling, which involved One-Hot Encoding, Label Encoding, and scaling of the data.

## 6. Modelling
Various modelling techniques were involved, with the aim of accessing the best model. The final model is the XGBoost, which had the best results, of all the other classifier models.

## 7. Conclusion and Recommendations
Lastly, following the analysis and modelling results, we drafted the solutions to the business problem that was previously defined.

## 8. Challenges 
The main challenge encountered was in the modelling section, where the model run time was high, especially when tuning the final model using GridSearchCV.