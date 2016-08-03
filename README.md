#Overview
This readme will walk you through the process of setting up a new instance of the Craft CMS running inside a Docker container. These instructions are a supplement to a Craft CMS workshop held at Clockwork (https://www.clockwork.com/).

#A. Install the Docker Toolbox
1. Download the Docker Toolbox: https://www.docker.com/products/docker-toolbox
2. Double click on the downloaded Docker Toolbox installation package.
3. The installation process will prompt you to **Choose a tool to get started with Docker**. Select **Docker Quickstart Terminal**. A terminal window will appear and perform some setup. Let it complete its process which may take 5 or 6 minutes.
4. You can click the **Continue** button on the **Install Docker Toolbox** application at any time, even if the terminal window is still processing.

#B. Install Xcode Command Line Tools
_Using a Terminal window._

1. `xcode-select --install`
2. Click the **Install** button.
3. You will see an error message stating the tools are already installed if they are in fact, already installed.

#C. Download and Install craftman
_Using a Terminal window._

1. `touch ~/.bash_profile`
2. `curl -o- https://raw.githubusercontent.com/gabrielmoreira/craftman/master/craftman_install | sh`
3. `source ~/.bash_profile`

#D. Create a New Craft CMS Container
_Using a Terminal window._

1. `cd Desktop`
2. `mkdir craft-docker && cd craft-docker`
3. `craftman --port=8080 install`
4. If a download or setup fails: `craftman -F -O -R install`

---

#About craftman
craftman is a tool for managing Craft CMS containers. It's Git repo can be found here: https://github.com/gabrielmoreira/craftman
