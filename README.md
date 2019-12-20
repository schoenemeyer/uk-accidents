## Mapping of Accidents using DBSCAN

This github is forked from João Paulo Figueira. My work was inspired by a great article on medium [1] from João .
It is a study on the UK accidents database. All I did was to add data for 2017 and 2018 and rerun the jupyter notebook.

My Testing Environment (Python2.7)
Python 2.7
scipy 1.2.1
numpy: 1.16.5
matplotlib: 2.2.3
statsmodels: 0.9.0
sklearn: 0.20.3
pandas: 0.23.4
geopandas: 0.6.2

My workstation: 1 x AMD FX-6300 6c with 1 x NVIDIA GTX 1050Ti running under CentOS 7.4, 32GB RAM
CUDA Driver 410.73 

## First test using DBSCAN

(1) uk-accident-map.ipynb

Clustering Data for one year typically takes roughly 12 sec wallclock; creating the list of cluster blobs takes typically a few seconds.

For this test UK RoadSafety Data were used from the link below [3]. 
You can run the notebook on multiple years or single years. The figure below shows the outcome for 6 years for a particular area in London    

<img src="https://github.com/schoenemeyer/uk-accidents/blob/master/figures/6years-uk-acc.PNG" width="580"> <img> 


You can also download the data from France [4] . You can use the fr-accident-map.ipynb. For the year 2018 you can focus on Paris and you will get this result:

<img src="https://github.com/schoenemeyer/uk-accidents/blob/master/figures/fr-2018.png" width="580"> <img> 


## Relevant Articles

[1] https://medium.com/@rawanme/u-k-traffic-accidents-data-analysis-10-years-c81293180ee5 2019

[2] https://towardsdatascience.com/mapping-the-uks-traffic-accident-hotspots-632b1129057b 2018

## Data Source with geolocations

# UK 
[3] RoadSafety Data UK (most recent data)
https://data.gov.uk/dataset/cb7ae6f0-4be6-4935-9277-47e5ce24a11f/road-safety-data, the same data you can find on kaggle (but not the most recent years) : https://www.kaggle.com/daveianhickey/2000-16-traffic-flow-england-scotland-wales

# France (ONISR)
[4] https://www.data.gouv.fr/en/datasets/base-de-donnees-accidents-corporels-de-la-circulation/    
Download caracteristiques-2018.csv

Other classifications are also under investigation 

https://medium.com/@rawanme/u-k-traffic-accidents-data-analysis-10-years-c81293180ee5

