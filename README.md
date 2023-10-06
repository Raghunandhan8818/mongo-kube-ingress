# Microservices in kubernetes
Simple Kubernetes-based app that contains 3 services:
1. Flask (Python) microservice (management of applications' logs)
2. Sinatra (Ruby) microservice (OAuth server - user registration and login)
3. MongoDB

The purpose of this app is to log history about web apps requests.

# See flask app routes for some more routes

## Features

1. Containerized microservices flask,sinatra.
2. Deployed to Kubernetes cluster see folder with kubernetes components.
3. Communication between microservices to resolve user's authentication
4. MongoDB storage
5. JWT authentication
6. Nginx proxy-server via Kubernetes Ingress

## How to run

1. To run in development follow instructions on how to build related docker images written in flask folder and sinatra folder.
2. In production follow Kubernetes official guide to deploy a cluster. Deploy all Kubernetes components from Kubernetes config folder for example via `kubectl apply -f <file>.yml`
