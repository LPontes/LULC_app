# LULC app

Classifies Land Use Land Cover in Brazil with Machine Learning and satellite images.
This application uses Sentinel-2 images and a Classification Tree algorithm to classify each image pixel on the main landcover classes in Brazil: 
- Water
- Bare soil
- Forest
- Annual crop
- Perennial crop
- Pasture
- Urban areas

## Instructions
- Step 1: Select the area you want to classify and draw a polygon with the tools on the map left bar
- Step 2: Check the box 'Use user-drawn AOI' and click "Submit" 
![app screenshot](./images/Screenshot_1.jpg)


## Development

The app uses a Classification Tree algorithm to predict landcover from Sentinel-2 image

To train the model data was colected as described on the 'retrieve_data' [notebook](https://github.com/LPontes/LULC_app/blob/master/notebooks/data_retrieve.ipynb).
- The data acquisicion process was taken using the Earth Engine python API and the geemap package

The modeling step can be found on [modeling.ipynb](https://github.com/LPontes/LULC_app/blob/master/notebooks/modeling.ipynb)

Deployment and hosting were acomplish with Heroku.
- The web app can be accessed on: [LULC_app](https://predict-land-cover-br.herokuapp.com/)



**warning:** This is a in progress project and there are improvements in the modeling process that are needed for a reliable result.

## Credits
- Google Earth Engine
- geemap
- Sentinel images
- Heroku



