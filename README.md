# Blender_Docker Project

## Introduction
The Blender Docker Project integrates Blender, a powerful open-source 3D creation suite, with Docker, a platform for containerization. This project aims to simplify and standardize Blender's deployment and usage across different systems and environments by packaging it into a Docker container.

## Purpose of the Blender Docker Project
#### Environment Independence:
Allows Blender to run seamlessly on any system with Docker support, eliminating installation issues.
#### Scalability:
Facilitates Blender usage in distributed computing setups for tasks like rendering.
#### Ease of Deployment:
Pre-configured Docker images reduce setup time and complexity.
#### Enhanced Collaboration:
Provides a standardized environment for teams working on 3D projects.

https://github.com/user-attachments/assets/6c5e91d8-5d8b-4d49-b944-6a1771e3215c

## Pre-requisites
A system with Docker installed and configured.

Basic knowledge of command-line tools.

## Steps
Pulling the Blender Docker Image

##### docker pull kasmweb/blender

## Running Blenderin a Container
Environment Variables
APP_ARGS - Additional arguments to pass to the application when launched.
Stand-alone Deployment
This image was designed to run natively within Kasm Workspaces, but it can also be deployed stand-alone and accessed through a web browser.

##### sudo docker run --rm -it --shm-size=512m -p 6901:6901 -e VNC_PW=password kasmweb/blender:1.16.0
The container is now accessible via a browser :
##### https://IP_OF_SERVER:6901

User : kasm_user
Password: password
Please note that some functionality, such as audio, uploads, downloads, and microphone pass-through, is only available when using Kasm Workspaces for orchestration.

## Conclusion
The Blender Docker Project successfully demonstrates the power of containerization in streamlining the deployment and usage of Blender, a versatile 3D creation suite. By leveraging Docker, the project ensures environment independence, scalability, and ease of deployment, enabling seamless operation across diverse systems.

The integration with Kasm Workspaces further enhances accessibility by providing a web-based interface, making Blender available through any modern browser. This flexibility, combined with features such as rolling updates and a standardized environment, makes the project ideal for both individual users and collaborative teams.

Through this project, we have bridged the gap between cutting-edge 3D design tools and modern containerization technology, offering a robust solution for distributed rendering, simplified setup, and enhanced collaboration. It sets a solid foundation for further innovation and integration in creative and technical workflows.
