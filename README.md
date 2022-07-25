# Домашнее задание к лекции «Docker»

Here is my homework for "Docker" lesson.
You require [Docker](https://docs.docker.com/engine/install/) to run.


## Clone this repo
```sh
git clone https://github.com/romanus1105/docker.git
```
# 1st task
## Build Custom NGINX Image
```sh
docker build -t webserver .
```
## Run Custom NGINX Image
```sh
docker run -it --rm -d -p 8080:80 --name web webserver
```
## Check webserver
Open your browser and navigate to http://localhost:8080 to make sure our html page is being served correctly.
# 2st task
## Build Django REST API service Image
```sh
docker build -t stock_products .
```
## Run Custom NGINX Image
```sh
docker run -it --rm -d -p 8000:8000 --name st_pr stock_products
```
## Check webserver
Open your browser and navigate to http://localhost:8000 to check REST API service with Django REST Client.
