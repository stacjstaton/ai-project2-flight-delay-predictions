# Predicting and Visualizing Flight Delays

## UNC AI/ML Bootcamp June 2024 Cohort

This project uses a public test dataset to create a machine learning (ML) model that can predict how likely a flight is to be delayed.

This dataset is from Kaggle and includes 539,383 datapoints from 40 United States international airports: [Airlines Dataset to predict a delay](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay).

The project team includes the following people: Stacy Magwano, Jenn Allen, Marques Oliver, Jack Kuppuswamy, and Vaughan Roberts.

[View our summary analysis presentation](https://docs.google.com/presentation/d/1j_SaOMO-UZ-eV1NtbN1Ck1CINe3boqKGDHTgbj5EA2c/edit#slide=id.p)

## How this Project is Structured

* /data: Contains the original source CSV (`Airlines.csv` and the processed CSVs)
* /data_processing: Contains the Jupyter Notebooks for data encoding, processing, and feature engineering. These create the two processed CSVs in the `data` folder.
* /tests: Contains test results showing accuracy and configuration for each AI/ML model.
* (root): Contains Juypter Notebooks for each model, visualizations, and an example (`example.ipynb`) for creating a new model with our processed data.

## Models and Algorithms

This project includes models that use these algorithms.

* [Adaptive Boosting](/ada_boost.ipynb)
* [Decision Tree](/decision_tree.ipynb)
* [Gradient Boosting](/gradient_boost.ipynb)
* KMeans
* KNN
* [Logistic Regression](/logistic_regression.ipynb)
* [Random Forest](/random_forest.ipynb)
* [Support Vector Machine](/svm.ipynb)
* [XGBoost](/xgboost.ipynb)

## Running this Project

All code is authored in Python within Jupyter Notebooks. You will need to be able to run the notebooks locally with an IDE like VSCode or with Google Collab.

## Findings and Additional Analysis

At present, the Random Forest model is most accurate, with an accuracy score of 66.2%. XGBoost came in at a close second at 65.7%.

While these accuracies are decent, the project team would like to further refine the models. This could include further refinement on the feature engineering and hyperparameter tuning.

## Dataset Documentation

### Target Variable

The `Delay` column is our target variable.

### Source Columns

* id (int): The index, included in the source dataset. We'll drop this since we want to use the index we define in our DataFrame.
* Airline (str): 2-letter code that corresponds to an airline name
* Flight (str): The flight ID
* AirportFrom (str): 3-letter code that corresponds to an airport name. Where the flight is going.
* AirportTo (str): 3-letter code that corresponds to an airport name. Where the flight is going.
* DayOfWeek (int): The numberic day of the week that the flight took place on
* Time (int): departure time measured in minutes from midnight (the range is 10-1439)
* Length (int): Duration of the flight in minutes
* Delay (int): Whether the flight was delayed or not. 0 or 1 value.

### Processed Columns

As part of data engineering, we encoded the columns and added some addition features.

Encoding. We encoded the `Time` and `Length` columns by ensuring they are integers and dividing them by 60 so that they represent hours.

New features. We used the encoded Time and Length columns to create features to track when a flight departed and when it arrived at its destination. We created groups for departures and arrivals as well.

### Airline Codes

The `Airline` column includes two letters to specify the airline. 

* Alaska Airlines: AS / ASA
* American Airlines: AA/AAL
* Air Canada: AC/ACA
* Aeromexico: AM / AMX
* Continental Airlines: CO / COA
* Delta Airlines: DL / DAL
* FedEx: FX / FDX
* Hawaiian Airlines: HA / HAL
* Northwest Airlines: NW / NWA
* Polar Air Cargo: PO / PAC
* Southwest Airlines: SW / SWA
* United Airlines: UA / UAL
* United Parcel (UPS): 5X / UPS
* Virgin Atlantic: VS / VIR
* VivaAerobús: VB / VIV
* WestJet: WS / WJ

### Airport Codes

The `AirportFrom` and `AirportTo` columns use three-letter codes to abbreviate the names.

* ATL - Hartsfield-Jackson Atlanta International Airport - Georgia
* AUS - Austin-Bergstrom International Airport - Texas
* BNA - Nashville International Airport - Tennessee
* BOS - Boston Logan International Airport - Massachusetts
* BWI - Baltimore-Washington International Thurgood Marshall Airport - Washington
* CLT - Charlotte Douglas International Airport - North Carolina
* DAL - Dallas Love Field - Texas
* DCA - Ronald Reagan Washington National Airport - Arlington, Virginia
* DEN - Denver International Airport - Colorado
* DFW - Dallas/Fort Worth International Airport - Texas
* DTW - Detroit Metropolitan Airport - Michigan
* EWR - Newark Liberty International Airport - New Jersey
* FLL - Fort Lauderdale–Hollywood International Airport - Florida
* HNL - Daniel K. Inouye International Airport - Honolulu, Hawaii
* HOU - William P. Hobby Airport - Houston, Texas
* IAD - Dulles International Airport - Virginia
* IAH - George Bush Intercontinental Airport - Houston, Texas
* JFK - John F. Kennedy International Airport - Queens, New York
* LAS - McCarran International Airport - Las Vegas, Nevada
* LAX - Los Angeles International Airport - California
* LGA - LaGuardia Airport - Queens, New York
* MCO - Orlando International Airport - Florida
* MDW - Chicago Midway International Airport - Illinois
* MIA - Miami International Airport - Florida
* MSP - Minneapolis–Saint Paul International Airport - Minnesota
* MSY - Louis Armstrong New Orleans International Airport - Louisiana
* OAK - Oakland International Airport - California
* ORD - O'Hare International Airport - Chicago, Illinois
* PDX - Portland International Airport - Oregon
* PHL - Philadelphia International Airport - Pennsylvania
* PHX - Phoenix Sky Harbor International Airport - Arizona
* RDU - Raleigh-Durham International Airport - North Carolina
* SAN - San Diego International Airport - California
* SEA - Seattle–Tacoma International Airport - Washington
* SFO - San Francisco International Airport - California
* SJC - Norman Y. Mineta San Jose International Airport - California
* SLC - Salt Lake City International Airport - Utah
* SMF - Sacramento International Airport - California
* STL - St. Louis Lambert International Airport - Missouri
* TPA - Tampa International Airport - Florida

## Dataset Documentation

* [Decision Tree](/README_DecisionTreeModel.md)