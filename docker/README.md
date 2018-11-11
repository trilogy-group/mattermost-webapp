# Dockerfile
 Dockefile is created on top of `node:10` image (debian).
 # Requirements
 - The project should be cloned from https://github.com/trilogy-group/mattermost-webapp
 - mattermost-server should be running (you can use the https://github.com/trilogy-group/mattermost-server -> master)
 - mattermost-server and mattermost-webapp should be siblings, start mattermost-server following the docker/README.md
 - You can run the client through mattermost-server Makefile (`make run`) or just adding the symlink `ln -nfs ../mattermost-webapp/dist client`
 - Docker version 18.06.0-ce
 - Docker compose version 1.22.0
  
# Quick Start
- Clone the repository
- Open a terminal session to that folder
- Run `docker/docker-cli start`
- Run `docker/docker-cli exec`
- At this point you must be inside the docker container, in the root folder of the project. From there, you can run the commands as usual:
	- `npm install` to install all dependencies
	- `make run` to start watcher and the frontend
	- `make stop` to kill all watchers
- When you finish working with the container, type `exit`
- Run `docker/docker-cli stop` to stop and remove the service.