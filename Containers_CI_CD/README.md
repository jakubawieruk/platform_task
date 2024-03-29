# Containers + CI/CD
## Build and run with Docker
Build image:
```
docker build -t shiny-docker .
```
If you're using an M-series Mac, you'll have to append the --platform linux/x86_64 tag when building the image.
```
docker build --platform linux/x86_64 -t shiny-docker .
```

Run the container with Docker:
```
docker container run -p 8180:8180 shiny-docker
```
