# Week 1: Introduction

## Introduction to GCP

GCP: Google Cloud Services

    Cloud storage
    

## Docker and docker-compose
Introduction to Docker

- Containers are isolated

    Why do we need Docker

    Creating a simple "data pipeline" in Docker

## Ingesting NY Taxi data to postgres

- postgres volumes
    to map files from local to the container


    Running Posgtres locally with Docker

    Using pgcli for connecting to the database

pgcli - command line for postgres

connecting to pg

pgcli -h localhost -p 5432 -u root -d ny_taxi
mycli -h localhost -p 5432 -u root -d ny_taxi


    Exploring the NY Taxi dataset
    
    Ingesting the data to the database
    
pgadmin docker

    Note if you have problems with pgcli, check this video for an alternative way to connect to your database


## Running Postgres locally with Docker
pgadmin docker

docker pull dpage/pgadmin4

winpty docker run -it \
  -e PGADMIN_DEFAULT_EMAIL="admin@admin.com" \
  -e PGADMIN_DEFAULT_PASSWORD="root" \
  -p 8080:80 \
  dpage/pgadmin4

enter to 
localhost:8080/browser

## Setting up infrastructure on GCP with Terraform
## Preparing the environment for the course
## Homework