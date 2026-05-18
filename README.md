# Sample App

This repository contains a sample Go application deployed using:

* Google Kubernetes Engine (GKE)
* Cloud Build
* Google Artifact Registry
* GitHub Triggers

## Branches

* `master` → Production deployment
* `dev` → Development deployment

## Deployment Flow

Cloud Build automatically:

1. Builds the Docker image
2. Pushes the image to Artifact Registry
3. Deploys the application to GKE

## Namespaces

* `prod`
* `dev`

## Files

* `cloudbuild.yaml` → Production pipeline
* `cloudbuild-dev.yaml` → Development pipeline
* `Dockerfile` → Container build configuration
* `main.go` → Application source code
