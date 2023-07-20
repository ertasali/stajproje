# README.md file

# This Project is designed for sending data over mqtt protocol and observing the data with the visualizer with the Grafana through from InfluxDB.

# This setup is for Windows users.

# Firstly, you need to install ubuntu from WSL to Windows operating system. 

# You need to use PowerShell for better. Here is the link that can provide information to install Ubuntu https://learn.microsoft.com/en-us/windows/wsl/install

# After the installation of ubuntu, in this project there are several programming tools that we going to use.

# The First programming tool is Node-Red. Node-Red is a flow-based, low-code development tool for visual programming developed originally by IBM for wiring together hardware devices, APIs and online services as part of the Internet of Things. Node-RED provides a web browser-based flow editor, which can be used to create JavaScript functions.

# To install Node-Red to your Windows here is the link https://nodered.org/docs/getting-started/windows

# After the installation of Node-Red, make sure you installed the "WSL 2 ubuntu" and after that The docker Desktop need to be installed. Here is the link that you can install through https://docs.docker.com/desktop/install/windows-install/

# After the installation of Docker, you need to connect from docker dektop to Ubuntu WSL 2. This is the path that you can do it. Docker Desktop -> Settings -> Resources -> WSL Integration -> Select UBUNTU.

# Now, the project installation can be start. If you are not using Visual Studio Code, I highly recommend it for this project and also in the future project of yours. Here is the link that you can install VS code https://code.visualstudio.com/download

# Firstly, open the VS code and from left down corner, connect to WSL UBUNTU and open the project that you download from the GitHub. Open a new terminal and make sure your directory is in the docker file. After that run this command "docker compose up" to create the whole volume of you project in the docker. 

# The installation needs to be started. If you are having trouble any kind make sure you did the all steps right.

# Here you go you can observe the project running from Docker Desktop.

# After that Firstly you can open Node-RED, InfluxDB and Grafana from the Docker Desktop and sign. 

# The Node-Red that you installed to your Windows system is for sending a data to the Node-Red that is on docker local host. Therefore, open Windows powershell and run this command "node-red" after that Go to your browser and type "localhost:1880" to enter the Node-Red that is sender.

# Finally you can use the MQTT in out functions in Node-Red and send the data to the docker project and from that node-red using influx function of Node-Red you can send the data to the InfluxDB and finally from there you can send it to the Grafana and get Visual of any kind of data.

