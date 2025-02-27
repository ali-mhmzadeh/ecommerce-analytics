# The Ecommerce Dashboard
This is a supporting repo to create analytical dashboard for the [Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) dataset by Kaggle. Current version provides a containarized platform to:  
1. Build a PostgreSQL database with Olist Ecommerce datasets. 
2. Build and initialize a local Superset instance with default username and password
3. Import a pre-made dashboard named Olist. 

The visualizations are backed by the open-source BI tool, [Apache-Superset](https://superset.apache.org/). Implementation is fully dockerized and can be reproduced in various environments. 

![2022-08-07 17-11-01](https://user-images.githubusercontent.com/59216368/183311249-cb96218a-19c6-4eea-b207-22932a861159.gif)



# Dependecies
You need to install docker and docker-compose prior to running containers.
You also need a Mapbox API key to provide basemap for your map visualizations. 
Get your free mapbox api from https://www.mapbox.com/.

# Installation
1. Clone this repo:
```
$ git clone https://github.com/ali-mhmzadeh/ecommerce-analytical-dashboard.git
```

2. Start dockerized services. PostgreSQL will run on ports 5433, just in case you already have Postgres running: 

```
$ cd ecommerce-analytical-dashboard
$ export MAPBOX_API_KEY = <YOUR-MAPBOX-API-KEY>
$ docker-compose up
```

# Quick start

1. Login to http://localhost:8080/login/ with the following credentials:
```
username: admin
password: 1234
```

2. Navigate to the Dashboards section and take a look at the olist dashboard. 






