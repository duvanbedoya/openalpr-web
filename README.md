# Openalpr Webservice in a docker container using Colombian Plates Recognition

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
curl -X POST -F "image=@carro12.jpg" http://`boot2docker ip`:8888/alpr
```
