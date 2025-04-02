# SIT737-2025-Prac5P: Dockerised LOOPII Application

This project demonstrates the containerisation of a simple Node.js web application using Docker and Docker Compose, as part of SIT737 Task 5.1P. The application displays a welcoming HTML page featuring a custom background and animated elements (like a dancing doll or running robot) for the LOOPII project.


## Application Features

- Serves a responsive HTML page via Express.js
  
- Displays a welcoming message with background and animated robot/doll
  
- Fully containerised using Docker
  
- Health check integrated using Docker Compose

## Tech Stack

- **Node.js** (v18)
  
- **Express.js** (Web server)
  
- **Docker**
  
- **Docker Compose**

## Project Structure

loopii-backend/ ├── public/ │ ├── background.jpg │ ├── doll.gif ├── index.js ├── package.json ├── Dockerfile └── docker-compose.yml

## How to Run Locally with Docker

### 1. Clone the Repository

git clone https://github.com/yourusername/sit737-2025-prac5p.git-->cd sit737-2025-prac5p

## Build and Run with Docker Compose
   
docker-compose up --build

Open the browser --> Visit: http://localhost:3040

## Dockerfile Overview

The Dockerfile performs the following:

--> Uses Node.js base image

--> Installs dependencies

--> Starts the Express server

## Docker Compose + Health Check

Docker Compose orchestrates the service and monitors it with a health check:

--> Automatically restarts if health check fails

--> Maps container port 3040 to your host

## Push to Docker Hub

docker tag image-name username/image-name:latest

docker push username/image-name:latest

docker push username/image-name:latest

View it at: https://hub.docker.com/repository/docker/username/image-name

## Preeth Ramadoss

## SIT737 – Cloud-Native Application Development

## Deakin University




