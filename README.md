# ai-project2-flight-delay-predictions

[todo - add project summary here]
 
## Dataset Documentation

This dataset is from Kaggle. [Airlines Dataset to predict a delay](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay)

#### Columns

- id (int): The index, included in the source dataset. We'll drop this since we want to use the index we define in our DataFrame.
- Airline (str): 2-letter code that corresponds to an airline name
- Flight [todo: add]
- AirportFrom [todo: add]
- AirportTo [todo: add]
- DayOfWeek [todo: add]
- Time: departure time measured in minutes from midnight (the range is 10-1439)
- Length: duration of the flight in minutes
- Delay: [todo: add]

#### Airline Codes

The `Airline` column includes two letters to specify the airline. 

- Alaska Airlines: AS / ASA
- American Airlines: AA/AAL
- Air Canada: AC/ACA
- Aeromexico: AM / AMX
- Continental Airlines: CO / COA
- Delta Airlines: DL / DAL
- FedEx: FX / FDX
- Hawaiian Airlines: HA / HAL
- Northwest Airlines: NW / NWA
- Polar Air Cargo: PO / PAC
- Southwest Airlines: SW / SWA
- United Airlines: UA / UAL
- United Parcel (UPS): 5X / UPS
- Virgin Atlantic: VS / VIR
- VivaAerobús: VB / VIV
- WestJet: WS / WJ

### Airport Codes

The `AirportFrom` and `AirportTo` columns use three-letter codes to abbreviate the names.

- ATL - Hartsfield-Jackson Atlanta International Airport - Georgia
- AUS - Austin-Bergstrom International Airport - Texas
- BNA - Nashville International Airport - Tennessee
- BOS - Boston Logan International Airport - Massachusetts
- BWI - Baltimore-Washington International Thurgood Marshall Airport - Washington
- CLT - Charlotte Douglas International Airport - North Carolina
- DAL - Dallas Love Field - Texas
- DCA - Ronald Reagan Washington National Airport - Arlington, Virginia
- DEN - Denver International Airport - Colorado
- DFW - Dallas/Fort Worth International Airport - Texas
- DTW - Detroit Metropolitan Airport - Michigan
- EWR - Newark Liberty International Airport - New Jersey
- FLL - Fort Lauderdale–Hollywood International Airport - Florida
- HNL - Daniel K. Inouye International Airport - Honolulu, Hawaii
- HOU - William P. Hobby Airport - Houston, Texas
- IAD - Dulles International Airport - Virginia
- IAH - George Bush Intercontinental Airport - Houston, Texas
- JFK - John F. Kennedy International Airport - Queens, New York
- LAS - McCarran International Airport - Las Vegas, Nevada
- LAX - Los Angeles International Airport - California
- LGA - LaGuardia Airport - Queens, New York
- MCO - Orlando International Airport - Florida
- MDW - Chicago Midway International Airport - Illinois
- MIA - Miami International Airport - Florida
- MSP - Minneapolis–Saint Paul International Airport - Minnesota
- MSY - Louis Armstrong New Orleans International Airport - Louisiana
- OAK - Oakland International Airport - California
- ORD - O'Hare International Airport - Chicago, Illinois
- PDX - Portland International Airport - Oregon
- PHL - Philadelphia International Airport - Pennsylvania
- PHX - Phoenix Sky Harbor International Airport - Arizona
- RDU - Raleigh-Durham International Airport - North Carolina
- SAN - San Diego International Airport - California
- SEA - Seattle–Tacoma International Airport - Washington
- SFO - San Francisco International Airport - California
- SJC - Norman Y. Mineta San Jose International Airport - California
- SLC - Salt Lake City International Airport - Utah
- SMF - Sacramento International Airport - California
- STL - St. Louis Lambert International Airport - Missouri
- TPA - Tampa International Airport - Florida