#Overview
This readme contains a set of instructions for creating a Docker container for an instance of the Craft CMS on Mac OS X. These instructions were supplement a Craft CMS workshop held at Clockwork (https://www.clockwork.com/).

These instructions will lead you through the following:

1. Setup of Docker
2. Setup of craftman
3. Configuration of a new Docker container for a new Craft CMS instance
4. Configuration of Craft

#Docker Setup
1. Download Docker: https://www.docker.com/products/docker#/mac
2. Copy Docker to your Applications folder
3. Start the Docker Application
4. The installation process will prompt Select **Docker Quickstart Terminal** and wait for the terminal session to complete (5 minutes)

#Docker Toolbox Setup
1. Download the Docker Toolbox: https://www.docker.com/products/docker-toolbox
2. Install the Docker Toolbox 

#About craftman
craftman is a tool for managing Craft CMS containers. It's Git repo can be found here: https://github.com/gabrielmoreira/craftman

#craftman Setup
1. Start a new **Terminal** window
1. `touch ~/.bash_profile`
2. `cd Desktop`
1. `mkdir craft-docker`
2. `cd craft-docker`
2. Download and install craftman: `curl -o- https://raw.githubusercontent.com/gabrielmoreira/craftman/master/craftman_install | sh`
4. Install Xcode Tools if requested
3. `source ~/.bash_profile`
5. `craftman --port=8080 install`
6. If a download or setup fails: `craftman -F -O -R install`

##Craft Setup
1. Click **Personal** on bottom of the admin page
3. Click **Try for free** in the Pro column