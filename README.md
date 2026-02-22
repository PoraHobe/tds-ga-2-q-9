# Docker Image Deployment

This project contains a simple Flask application and a GitHub Actions workflow to build and push a Docker image to Docker Hub.

## Prerequisites

1. **Docker Hub Account**: You need a Docker Hub account.
2. **GitHub Secrets**: Add the following secrets to your GitHub repository:
    * `DOCKER_USERNAME`: Your Docker Hub username.
    * `DOCKER_PASSWORD`: Your Docker Hub password or access token.

## Instructions

1. **Commit and Push**:
    * The workflow is configured to run on pushes to the `main` branch.
    * Commit your changes and push to `main` to trigger the build and push process.

2. **Verify Deployment**:
    * Once the workflow completes successfully, check your Docker Hub repository.
    * You should see an image named `q-docker-hub-image` with the tag `24f2008474`.

## Image URL

The Docker image URL will be in the format:
`https://hub.docker.com/repository/docker/<DOCKER_USERNAME>/q-docker-hub-image/general`

If you need to provide a specific format for verification (e.g., with a token):
`https://hub.docker.com/repository/docker/<DOCKER_USERNAME>/q-docker-hub-image/general?secret=<TOKEN>&identifier=<DOCKER_USERNAME>`
