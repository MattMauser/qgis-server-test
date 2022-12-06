# Getting Started
To start using this with docker compose, navigate to the folder and run the command
`docker-compose up` 
This will download the necessary images and will run the application.

## QGIS Server
The QGIS Server will be running and accessed through the nginx server on the port 8010. There has already been an OttawaArea.qgs QGIS project created with the required data / shapefiles to create a test WMS service. The service can be reached through the URL:
[http://localhost:8010/ogc/OttawaArea?request=GetCapabilities&service=WMS](http://localhost:8010/ogc/OttawaArea?request=GetCapabilities&service=WMS)

## Maproxy Server
The mapproxy server currently isn't able to connect to the QGIS Server and has it's connection refused. I figure this is probably an issue with the NGINX configuration (found in conf/nginx.conf).
That being said, you can reach the Mapproxy site through [http://localhost:8080/demo](http://localhost:8080/demo).
