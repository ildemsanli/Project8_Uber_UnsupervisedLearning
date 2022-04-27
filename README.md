![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Project | Module 3 - Supervised Machine Learning 

## Authors
### Vito Coquet & Ildem Sanli 

## Introduction

The goal of this project is to practise unsupervised learning using Uber data. Our aim is to create clusters of Uber pick-ups for April 2014 data. Additionally, we implement the same models using September 2014 data to be able to compare our results with other groups.   

## About the Dataset

A dataset of 564516 rows and 5 columns containing longitude, latitude, date and base information of Uber pick-ups in April 2014. 


## Data Preparation and EDA 

We created a hour and a weekday column for our EDA and dropped the date/time column. 
We first lokked into hourly and daily distribution of pick-ups.
For our analysis, we split the times of the day into morning, afternoon, evening and night and plottes the distribution of pick-ups according to the time of the day and also according to the base. 

## Models 

We used the following models :

-K-means Clustering : K-means algorithm clusters data by separating samples in a given number of groups of equal variance. We first identified the number of clusters using Kelbow visualizer and then clustered tha data accordingly. 

-DBSCAN : expands clusters starting from samples with similar density. It does not require a specific cluster number to be given. 

-OPTICS : works similarly to DBSCAN, more suitable for larger datasets.

-Agglomerative Clustering :  each observation starts in its own cluster, and clusters are successively merged together, requires cluster number.

We obtained the best results with DBSCAN and showed these data on a folium map. 

## Repo Structure

Our repo is organised as follows:

Data: Original and cleaned datasets in CSV format (April and September)

Code: Data preparation and Model Implementation

Images: The images of the plots we obtained usign different methods of clustering and folium map.
