#Overview
This readme will walk you through the process of setting up a new instance of the Craft CMS running inside a Docker container. These instructions are a supplement to a Craft CMS workshop held at Clockwork (https://www.clockwork.com/).

#A. Setup Docker
1. Download the Docker Toolbox: https://www.docker.com/products/docker-toolbox
2. Double click on the downloaded Docker Toolbox installation package.
3. The installation process will prompt you to **Choose a tool to get started with Docker** Select **Docker Quickstart Terminal**. A terminal window will appear and perform some setup. Let it complete its process which may take 5 or 6 minutes.
4. You can click the **Continue** button on the **Install Docker Toolbox** application at any time, even if the terminal window is still processing.

#B. Setup craftman
1. Start a new **Terminal** window
2. $ `touch ~/.bash_profile`
3. $ `cd Desktop`
4. $ `mkdir craft-docker && cd craft-docker`
5. Download and install craftman: $ `curl -o- https://raw.githubusercontent.com/gabrielmoreira/craftman/master/craftman_install | sh`
6. Install Xcode Tools if requested, this will happen if Git is not installed, and then re-run the install craftman command.
7. $ `source ~/.bash_profile`

#C. Create new Craft CMS Container
1. $ `craftman --port=8080 install`
2. If a download or setup fails: $ `craftman -F -O -R install`

##C. Craft Setup
1. Click **Personal** on bottom of the admin page
2. Click **Try for free** in the Pro column

---

#About craftman
craftman is a tool for managing Craft CMS containers. It's Git repo can be found here: https://github.com/gabrielmoreira/craftman
