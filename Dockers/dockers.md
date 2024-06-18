# What is Docker?
Docker is a software platform that employs OS virtualisation, enabling IT organisations to swiftly generate, deploy, and execute applications within Docker containers.

These containers encapsulate all the necessary dependencies, including, libraries, and binaries, making the, lightweight ro self-making them, lightweight and self sufficient.

# Docker vs Venv
* Docker operates with a Docker Engine layer, whereas Venv functions with Hypervisor layer. 
* Docker envs maintain low memory usage, venvs consume a high amount of memory
* Dockers deliver high performance due to its single docker engine. Venvs tend to suffer when multiple instance are running on a server leading to poorer performance. 
* Dockers are portable. 
* Uses YAML format


# How does Docker work?

The docker engine comprises of two components, a server and a client. Which communicate through a REST API.

The server conveys instructions to the client. 

# Components of Dockers
* Docker client and server
* Docker Image
* Docker Registry
* Docker Container