# LULC_app

Classifies Land Use Land Cover in Brazil with Machine Learning and satellite images.

## Instructions
![app screenshot](./images/Screenshot_1.jpg)


## Development

The app uses a Classification Tree algorithm to predict landcover from Sentinel-2 image

To train the model data was colected as described on the 'retrieve_data' notebook.
- The data acquisicion process was taken using the Earth Engine python API and the geemap package
- 
The modeling step can be found on notebook/modeling.ipynb

Deployment and hosting were acomplish with Heroku.
- The web app can be accessed on: [LULC_app](https://predict-land-cover-br.herokuapp.com/)



* warning: This is a in progress project and there are improvements in the modeling process that are needed for a reliable result.

## Credits
- Google Earth Engine
- geemap
- Sentinel images



