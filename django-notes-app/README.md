# Simple Notes App for TWS Community
This is a simple notes app built with React and Django.

## About This Project

A Django-based notes application containerized using Docker.


## Requirements
1. Python 3.9
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/LondheShubham153/django-notes-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`

## What I learned
- Building Docker images for Python/Django apps
- Running Django inside containers
- Managing dependencies using requirements.txt


## Credits

This project was built while following a Docker tutorial by TrainWithShubham (YouTube).

