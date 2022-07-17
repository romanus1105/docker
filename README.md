# Домашнее задание к лекции «Docker»

Here is my homework for "Docker" lesson.
You requires [Docker](https://docs.docker.com/engine/install/) to run.

## Clone this repo
Install the dependencies and run:
```sh
git clone https://github.com/romanus1105/docker.git
```
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
