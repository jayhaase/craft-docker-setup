#Overview
This readme will walk you through the process of setting up a new instance of the Craft CMS running inside a Docker container. These instructions are a supplement to a Craft CMS workshop held at Clockwork (https://www.clockwork.com/).

This readme covers the following high-level steps:

1. Setup of Docker
2. Setup of craftman
3. Creation of a Docker container for a new Craft CMS instance
4. Configuration of Craft

#Docker Setup
1. Download the Docker Toolbox: https://www.docker.com/products/docker-toolbox
2. Double click on the downloaded Docker Toolbox installation package.
4. The installation process will prompt you to **Choose a tool to get started with Docker** Select **Docker Quickstart Terminal**. A terminal window will appear and perform some setup. Let it complete its process which may take 5 or 6 minutes.
5. You can click the **Continue** button on the **Install Docker Toolbox** application at any time, even if the terminal window is still processing.

#craftman Setup
1. Start a new **Terminal** window
1. $ `touch ~/.bash_profile`
2. $ `cd Desktop`
1. $ `mkdir craft-docker && cd craft-docker`
2. Download and install craftman: $ `curl -o- https://raw.githubusercontent.com/gabrielmoreira/craftman/master/craftman_install | sh`
4. Install Xcode Tools if requested, this will happen if Git is not installed, and then re-run the install craftman command.
3. $ `source ~/.bash_profile`
5. $ `craftman --port=8080 install`
6. If a download or setup fails: $ `craftman -F -O -R install`

##Craft Setup
1. Click **Personal** on bottom of the admin page
3. Click **Try for free** in the Pro column

---

#About craftman
craftman is a tool for managing Craft CMS containers. It's Git repo can be found here: https://github.com/gabrielmoreira/craftman
