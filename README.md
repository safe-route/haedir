# Háedir

Project documents, central documentation and artifacts.

## Table of Contents

- [Háedir](#háedir)
  - [Table of Contents](#table-of-contents)
  - [Team C22-PS305](#team-c22-ps305)
  - [Overview](#overview)
  - [How to navigate](#how-to-navigate)
  - [Project Artifacts](#project-artifacts)
- [Documentation](#documentation)
- [Android Path](#android-path)
  - [Overview](#overview-1)
  - [Library](#library)
  - [Installation](#installation)
  - [Structure](#structure)
  - [MVVM Architecture Pattern](#mvvm-architecture-pattern)
  - [Room Database](#room-database)
  - [Api](#api)
  - [Feature](#feature)
  - [Known Issue](#known-issue)
  - [Reference](#reference)
- [Cloud Computing Path](#cloud-computing-path)
      - [For a Bird Eye View of the API Docs Go Here](#for-a-bird-eye-view-of-the-api-docs-go-here)
  - [Overview](#overview-2)
- [Machine Learning Path](#machine-learning-path)
  - [Overview](#overview-3)
  - [Clustering](#clustering)
    - [Model Description](#model-description)
    - [Model generation](#model-generation)
    - [Centroid](#centroid)
    - [Statistic](#statistic)
  - [Habit Tracker](#habit-tracker)
    - [Model Description](#model-description-1)
    - [Model Generation](#model-generation-1)
    - [Model](#model)
    - [Flask](#flask)
  - [Known Issues](#known-issues)
  - [Research and Paper Source](#research-and-paper-source)

## Team C22-PS305

* M2002F0101 - Christopher Chandrasaputra
* M2006F0613 - Hanif Adam Al Abraar
* A2183F1771 - Fillah Akbar Firdausyah
* A2009J0968 - Ikhsan Cahya Mardika 
* C2009F0967 - I Putu Cahya Adi Ganesha
* C2306G2617 - Muhammad Anggi Wirahmat

## Overview

This is the central project visibility repository, providing you with a high-level overview of the project safe route. For a deeper overview of the project please refer to the respective project in the group.

## How to navigate

1. To see the product backlog in GitLab go to issues in the side bar and choose board to see the **Kanban Board**
2. Keep scrolling this view to find the link to various project artifacts (open with **Bangkit Academy Organization Account**)

## Project Artifacts

- Project Charter: https://docs.google.com/document/d/1aKTBomEo987yg4Kh0ns9HKky2CiLXA0OSbOcVf8WhWY/edit?usp=sharing
- Project Schedule: https://docs.google.com/spreadsheets/d/119f0Df_cexx2XERhFKch1P9jZyjw3M7L/edit?usp=sharing&ouid=108000726898413588789&rtpof=true&sd=true
- Infrastructure (subject to change): https://drive.google.com/file/d/1-sSHtzpbLx0dG5DKdmQhJDaWeBk8oNLR/view?usp=sharing
- Risk Management Documents: https://docs.google.com/document/d/1M5otteETpyKzQ8FUmXFmE--7y0xWhPg1/edit?usp=sharing&ouid=108000726898413588789&rtpof=true&sd=true
- OKRs: https://docs.google.com/document/d/1Y7cj9sI6R5-Oswl3LwKtFmsa2ZlrOi7Fu2AdM9_Va_k/edit?usp=drivesdk
- Questions compilations: https://docs.google.com/document/d/19-62w-kBfKQ3oxC48K3GisvmXC926CxO1NuXsO6qw4E/edit?usp=drivesdk
- Mentoring sheet: https://docs.google.com/document/d/1D3n3aSPo53AXyQhA_2vRIMWpK0t2XVru5b5_l6M-hCs/edit?usp=drivesdk
- Sprint Backlog: To Be Added or not...
- Figma: https://www.figma.com/file/Cn9PFgj1dZV0VYGosjn1tx/Safe-Route?node-id=0%3A1
- List of Question: https://docs.google.com/document/d/19-62w-kBfKQ3oxC48K3GisvmXC926CxO1NuXsO6qw4E/edit?usp=sharing

# Documentation

Central repository documentation for each learning path.

# Android Path

Safe route android app build with kotlin to comunicate with our technology

## Overview

- [Library](#library)
- [Installation](#installation)
- [Structur](#structur)
- [Architecture Pattern](#mvvm-architecture-pattern)
- [Api](#api)
- [Feature](#feature)
- [Known Issue](#known-issue)
- [Reference](#reference)

## Library

in this app we use library such as:

- [Retrofit](https://github.com/square/retrofit)
- [Circle Image View](https://github.com/hdodenhof/CircleImageView)
- [Glide](https://github.com/bumptech/glide)
- [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart)
- [Android Jetpack](https://developer.android.com/jetpack)

## Installation

Note: Before installing this project to your machine make sure minimum you have installed [Android Studio Bumblebee (2021.1.1) Stable](https://android-developers.googleblog.com/2022/01/android-studio-bumblebee-202111-stable.html)

```
git clone https://gitlab.com/safe-route/android-app.git
```

then sync the Graddle or Build > Rebuild Project

## Structure

No definite structure for this project, this is just basic Android Project Structure. go to `mainpackage`.
to access the google maps service, Edit `AndroidManifest.xml` and then place your Google Map Api Key. and also place your Google Map Api Key to this line code `buildConfigField("String", "API_KEY", '"PlAcEYouRAPIkeYHeRE"')` in the Graddle file.

## MVVM Architecture Pattern
![mvvm](https://gitlab.com/safe-route/android-app/-/blob/main/Image/mvvm.png)
This project use mvvm patern for easly to maintain and organizing code.

## Room Database
For costumize the database go to `mainpackage/database/DataRoomDatabase.kt`
`@Database(entities = [DataTraining::class, DataPredict::class], version = 1)`
and update the version

## Api
Note: To use your API go to the folder `mainpackage/api` then customize according to your needs

## Feature

- Statistic
  ![alt text](https://gitlab.com/safe-route/android-app/-/blob/main/Image/home-screen.png)
  ![alt text](https://gitlab.com/safe-route/android-app/-/blob/main/Image/detail-statistic.png)

- Map
  ![alt text](https://gitlab.com/safe-route/android-app/-/blob/main/Image/map-screen.png)
  ![centroid](https://gitlab.com/safe-route/android-app/-/blob/main/Image/centroid-danger-screen.png)
  ![routing](https://gitlab.com/safe-route/android-app/-/blob/main/Image/routing-screen.png)

- Report
  ![report crime](https://gitlab.com/safe-route/android-app/-/blob/main/Image/report-sreen.png)

## Known Issue
- Handle background service efficiently
- Versioning Roomdatabase
- UI/UX

## Reference

- [https://developer.android.com/kotlin](https://developer.android.com/kotlin)
- [https://developers.google.com/maps/documentation/android-sdk](https://developers.google.com/maps/documentation/android-sdk)

# Cloud Computing Path

#### For a Bird Eye View of the API Docs Go [Here](https://gitlab.com/safe-route/cloud-computing/gcp-endpoints)

## Overview

1. [calculate_trigger_function](https://gitlab.com/safe-route/cloud-computing/calculate_trigger_function).
2. [cloud-shell-script](https://gitlab.com/safe-route/cloud-computing/cloud-shell-script).
3. [clustering-from-bq](https://gitlab.com/safe-route/cloud-computing/clustering-from-bq)
4. [clustering-job](https://gitlab.com/safe-route/cloud-computing/clustering-job)
5. [front-facing-website](https://gitlab.com/safe-route/cloud-computing/front-facing-website)
6. [get_subdistrict_stat](https://gitlab.com/safe-route/cloud-computing/get_subdistrict_stat)
7. [json-to-firestore](https://gitlab.com/safe-route/cloud-computing/json-to-firestore)
8. [parse-to-bigquery-table](https://gitlab.com/safe-route/cloud-computing/parse-to-bigquery-table)
9. [return_all_subdistrict_coord](https://gitlab.com/safe-route/cloud-computing/return_all_subdistrict_coord)
10. [saferoute-jwt-express](https://gitlab.com/safe-route/cloud-computing/saferoute-jwt-express)
11. [service-composer](https://gitlab.com/safe-route/cloud-computing/services-composer)
12. [valhalla-server](https://gitlab.com/safe-route/cloud-computing/valhalla-server)
13. [web-app-sandbox](https://gitlab.com/safe-route/cloud-computing/web-app-sandbox)

# Machine Learning Path

## Overview

* **[Clustering](#clustering)**
* **[Habit Tracker](#habit-tracker)**
* **[Known Issues](#known-issues)**
* **[Team](#team)**

## Clustering

### Model Description

Clustering model is produced using scikit-learn DBScan class. Centroid comes from the average of each cluster with the range is the maximum distance of centroid to one of cluster members.

### Model generation

- Model : Use create_model() method
- Statistic : Use generate_area_statistic(data) with data being the DataFrame of csv file

### Centroid
JSON File Format
```
{
    "centroids": [
        {
            "id": ... (int),
            "latitude": ... (float),
            "longitude": ... (float),
            "range": ... (float),
            "crime_info": {
                <crime_type>(string): ... (int),
                ...
            }
        },
        ...
    ]
}
```

### Statistic
JSON File Format
```
{
    "statistic": [
        "subdistrict": ... (string),
        "total_crime": ... (int),
        "crime_info": {
            <crime_type>(string): ... (int),
            ...
        }
        "coordinates": ... (list of* float)
    ]
}
```
Statistic JSON File Note:
- coordinates list order is latitude, longitude
- list may contain another list
- please take a look at area_statistic.json before use


## Habit Tracker

### Model Description

Habit tracker model is created for each user that use the application, it utilize LSTM mechanics to predict multivariate multilabel time series data. Model will be fed with multiple inputs which is date, time, and location. The model will give location (latitude and longitude) as output.

### Model Generation

User's model will be generated when the endpoint ```/create``` called with username as URL parameters*.

\* further endpoint detail will be given [below](#flask)

### Model
```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 lstm (LSTM)                 (None, 15, 64)            18176     
                                                                 
 lstm_1 (LSTM)               (None, 15, 32)            12416     
                                                                 
 lstm_2 (LSTM)               (None, 16)                3136      
                                                                 
 flatten (Flatten)           (None, 16)                0         
                                                                 
 dense (Dense)               (None, 16)                272       
                                                                 
 dense_1 (Dense)             (None, 8)                 136       
                                                                 
 dense_2 (Dense)             (None, 2)                 18        
                                                                 
=================================================================
Total params: 34,154
Trainable params: 34,154
Non-trainable params: 0
_________________________________________________________________
```
* Model input shape=(15, 6)
* Model input data columns:

| column      | type    | range          | description              |
|-------------|---------|----------------|--------------------------|
| year        | integer |        *       | year timestamp           |
| month       | integer |     1 - 12     | month timestamp          |
| day_of_week | integer |      1 - 7     | day of week              |
| time        | integer |    0 - 1440    | cumulative minute of day |
| latitude    |  float  |  -90.0 - 90.0  | latitude                 |
| longitude   |  float  | -180.0 - 180.0 | longitude                |

* Model output:

| column    | type  | range          | description |
|-----------|-------|----------------|-------------|
| latitude  | float |  -90.0 - 90.0  | latitude    |
| longitude | float | -180.0 - 180.0 | longitude   |

### Flask
url: https://model-ck44nnq7hq-as.a.run.app

| endpoint  | url_param        | body           | method |
|-----------|------------------|----------------|--------|
| /create   | username(string) |        -       | GET    |
| /train    | username(string) | json-object-1* | POST   |
| /forecast | username(string) | json-object-2* | POST   |

\* refer to the format below

* json-object-1
```
{
	"username": ...,
	"data": [
	        {
	            "datetime": ...,
	            "latitude": ...,
	            "longitude": ...
	        },
	        ...
	        {
	            "datetime": ...,
	            "latitude": ...,
	            "longitude": ...
	        }
	    ]
}
```

* json-object-2
```
{
	"username": ...,
    "email": ...,
    "latitude": ...,
	"longitude": ...,
	"data": [
	        {
	            "datetime": ...,
	            "latitude": ...,
	            "longitude": ...
	        },
	        ...
	        {
	            "datetime": ...,
	            "latitude": ...,
	            "longitude": ...
	        }
	    ]
}
```
* json key-value description

| key       | value                | range                     |
|-----------|----------------------|---------------------------|
| username  |        string        |             -             |
| email     |        string        |             -             |
| latitude  |         float        |        -90.0 - 90.0       |
| longitude |         float        |       -180.0 - 180.0      |
| data      | json-array-of-object |             -             |
| datetime  |       timestamp      | %yyyy/%mm/%dd %hh:%MM:%ss |

## Known Issues

* Clustering - Require real data from local authorities
* Habit Tracker - Model architecture has not yet been optimized
* Habit Tracker - Costly data and model pipelining
* Habit Tracker - Require a lots of data to create optimum model


## Research and Paper Source

- E. Eck, Chainey, G. Cameron, Leitner, E. Wilson. "Mapping Crime: Understanding Hot Spots". NIJ Special Report (2005): 0-77.
