# Getting Started
To start using this with docker compose, navigate to the folder and run the command
`docker-compose up` 
This will download the necessary images and will run the application.

## QGIS Server
The QGIS Server will be running and accessed through the nginx server on the port 8010. There has already been an OttawaArea.qgs QGIS project created with the required data / shapefiles to create a test WMS service. The service can be reached through the URL:
[http://localhost:8010/ogc/OttawaArea?request=GetCapabilities&service=WMS](http://localhost:8010/ogc/OttawaArea?request=GetCapabilities&service=WMS)

## Mapproxy Server
You can reach the Mapproxy site through [http://localhost:8080/demo](http://localhost:8080/demo). This can be configured by changing the mapproxy/mapproxy.yaml config file.

[http://localhost:8080/service?Request=GetCapabilities](http://localhost:8080/service?Request=GetCapabilities) is the link to the WMS GetCapabilities page. More access options can be seen in the mapproxy.yaml file.
