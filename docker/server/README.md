# Docker
## Conductor server
This Dockerfile create the conductor:server image

## Building the image
`docker build -t conductor:server .`

## Running the conductor server
 - Standalone server (interal DB): `docker run -p 8080:8080 -d -t conductor:server`
 - Server (external DB required): `docker run -p 8080:8080 -d -t -e "CONFIG_PROP=config.properties" conductor:server`
