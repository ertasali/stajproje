# README.md

This Project is designed for sending data over mqtt protocol and observing the data with the visualizer with the Grafana through from InfluxDB.

## This setup is for Windows users.

Firstly, you need to install ubuntu from WSL to Windows operating system. 

You need to use PowerShell for better experience. Here is the link that can provide information to install Ubuntu https://learn.microsoft.com/en-us/windows/wsl/install

## Ubuntu in Powershell or Command Prompt

```bash
wsl --install
```
## Check version

```bash
wsl -l -v
```
## Set version to WSL 2

```bash
wsl --set-default-version 2
```
## If installed previous Upgrade version

```bash
wsl --set-default-version 2
```

## After the installation of WSL

Now the subsystem for Linux(WSL) can be installed.

## In a Powershell terminal you can run:

```bash
wsl --list --online
```
to see all available distros.

## Install Ubuntu-20.04

```bash
wsl --install -d Ubuntu-20.04
```
After the installation the prompt will be open.

## Check

```bash
wsl -l -v
```
## Node-RED

The First programming tool is Node-Red. Node-Red is a flow-based, low-code development tool for visual programming developed originally by IBM for wiring together hardware devices, APIs and online services as part of the Internet of Things. Node-RED provides a web browser-based flow editor, which can be used to create JavaScript functions.

## To install Node-Red to your Windows:

Using Powershell:
```bash
node --version; npm --version
```
Using cmd:
```bash
 node --version && npm --version
```
You should recieve an output looks similar to:
```bash
v18.15.0
9.5.0
```
## Install Node-RED

```bash
npm install -g --unsafe-perm node-red
```
## Run Node-RED

```bash
C:>node-red
```
## Open Node-RED
http://localhost:1880


After the installation The docker Desktop need to be installed. Here is the link that you can install through https://docs.docker.com/desktop/install/windows-install/

After the installation of Docker, you need to connect from docker desktop to Ubuntu WSL 2. This is the path that you can do it.
```
Docker Desktop -> Settings -> Resources -> WSL Integration -> Select UBUNTU.
```
## Project

 Now, the project installation can be start. If you are not using Visual Studio Code, I highly recommend it for this project and also in the future project of yours. Here is the link that you can install VS code https://code.visualstudio.com/download

## Firstly:
 Open the VS code and from left down corner, connect to WSL UBUNTU and open the project that you download from the GitHub.
 
Open a new terminal and make sure your directory is in the docker file. After that run this command:

## In terminal of VS that is working in WSL:
```bash
docker compose up
```

"docker compose up" is to create the whole volume of you project in the docker. 

The installation needs to be started. If you are having trouble any kind make sure you did the all steps right.

## Final

Here you go you can observe the project running from Docker Desktop.

## Usage

You can open Node-RED, InfluxDB and Grafana from the Docker Desktop and sign. 

The Node-Red that you installed to your Windows system is for sending a data to the Node-Red that is on docker local host. Therefore, open Windows powershell and run this command "node-red" after that Go to your browser and type "localhost:1880" to enter the Node-Red that is sender.

Finally you can use the MQTT in out functions in Node-Red and send the data to the docker project and from that Node-RED using influxdb function of Node-Red you can send the data to the InfluxDB and finally from there you can send it to the Grafana and get Visualized data.

