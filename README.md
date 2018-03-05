# Openalpr Webservice in a docker container trained with Colombian Plates

This is a simple docker container  configured using only  first step of training (train-ocr) you only need clone repository and  build it to get 
a docker image.

## To Build

```
docker build -t openalpr-web .
```

## To Run

```
docker run -d -p 8888:8888 openalpr-web
```

## To Test

```
curl -X POST -F "image=@carro12.jpg" http://0.0.0.0:8888/alpr
```

