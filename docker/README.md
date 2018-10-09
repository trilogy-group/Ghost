# Dockerfile
 Dockefile is created on top of `node:carbon` image.
 # Requirements
 - The project should be cloned from https://github.com/trilogy-group/Ghost
 - Docker version 18.06.0-ce
 - Docker compose version 1.22.0
  
# Quick Start
- Clone the repository
- Open a terminal session to that folder
- Run `docker/docker-cli start`
- Run `docker/docker-cli exec`
- At this point you must be inside the docker container, in the root folder of the project. From there, you can run the commands as usual:
	- `yarn setup` to first-time setup & install tasks.
	- `grunt dev` to start Ghost.
	- `grunt test-all` to run tests.
	
- When you finish working with the container, type `exit`
- Run `docker/docker-cli stop` to stop and remove the service.
 