# docker-tempered [![Docker Pulls](https://img.shields.io/docker/pulls/gutmensch/tempered.svg)](https://registry.hub.docker.com/u/gutmensch/tempered/)

TEMPered is a temperature and humidity querying daemon compatible with some cheap devices from your favorite sale spot. It has been created and maintained by edorfaus (see https://github.com/edorfaus/TEMPered/ for more info). This image is basically targeted for the QNAP docker container station, but it should work everywhere. Make sure to connect your USB device from the host to the container with the --device parameter. The container sends temperature and humidity data to a predefined graphite url.

## Usage
```
docker pull gutmensch/tempered
docker run --device=/dev/ -ti gutmensch/tempered start.sh
```

## Misc
To support newer devices this image applies some pull requests, which have not been merged (yet). The project itself looks a bit abandoned.
