# Deploying a service in Yandex DataSphere from a Docker image with FastAPI

This example features a basic Docker image built on the FastAPI framework for deploying a service in Yandex DataSphere. The service implements image health checks and reports metrics in Prometheus format.

## Building a Docker image

Install Docker. In the command shell, run the following commands:

```
docker build --platform linux/amd64 -t fastapi-docker .
docker tag fastapi-docker <docker_repo_with_tag>
docker push <docker_repo_with_tag>
```

For details, see [this step-by-step guide](https://yandex.cloud/docs/datasphere/tutorials/node-from-docker-fast-api) in the Yandex Cloud documentation.
