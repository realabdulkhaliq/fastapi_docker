## Default Compose YAML/YML file

name: fastapi_docker_compose
services:
fastapi_docker_compose:
build:
context: D:\fastapi_docker\hicompose
dockerfile: Dockerfile
container_name: fastapi_docker_container
image: fastapi_docker_compose
networks:
default: null
ports: - mode: ingress
target: 8000
published: "8000"
protocol: tcp
networks:
default:
name: fastapi_docker_compose_default
