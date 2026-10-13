# Docker Networking with Multiple Containers

## Objective
To understand Docker networking concepts and configure a multi-container application using a custom bridge network.

## Technologies Used
- Docker
- Python
- Flask
- MySQL
- Redis

## Project Overview
This project demonstrates how multiple Docker containers communicate with each other using a custom bridge network. A Flask REST API runs in one container, MySQL runs in another, and Redis provides caching.

## Implementation Steps
1. Created a custom bridge network named `my-bridge-net`.
2. Verified the network using `docker network ls`.
3. Inspected network configuration using `docker network inspect my-bridge-net`.
4. Created a Flask REST API using Python.
5. Built the Flask Docker image.
6. Launched the Flask, MySQL, and Redis containers on the same network.
7. Tested container connectivity using container names.
8. Verified that the Flask API works at `http://localhost:5001/about`.

## Files
- `app.py` — Flask REST API.
- `Dockerfile` — Instructions to build the Flask image.
- `requirements.txt` — Python dependencies.

## Key Learnings
- Creating and inspecting Docker bridge networks.
- Running multiple containers.
- Communicating between containers using container names.
- Exposing container ports to the host using port mapping.
- Checking container status and connectivity.

## Conclusion
The experiment demonstrates Docker bridge networking and communication between multiple containers. The Flask application can be accessed through the mapped host port, while the containers can communicate using their names on the shared network.
