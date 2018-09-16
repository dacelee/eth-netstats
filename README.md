Moac Network Stats
============


This is a visual interface for tracking moac network status. It uses WebSockets to receive stats from running nodes and output them through an angular interface. It is the front-end implementation for [moac-netstats-api](https://github.com/).


## Prerequisite
* node
* npm

## Installation
Make sure you have node.js and npm installed.
```bash
sudo apt-get update
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.32.1/install.sh | bash
source ~/.bashrc
nvm install v6.9.1
```
Clone the repository and install the dependencies

```bash
git clone https://github.com/dacelee/moac-netstats/
cd moac-netstats
npm install
sudo npm install -g grunt-cli
```

##Build the resources
NetStats features two versions: the full version and the lite version. In order to build the static files you have to run grunt tasks which will generate dist or dist-lite directories containing the js and css files, fonts and images.


To build the full version run
```bash
grunt
```

To build the lite version run
```bash
grunt lite
```

If you want to build both versions run
```bash
grunt all
```

##Run

```bash
npm start
```
see the interface at http://localhost:3000
##set up Port of WS_SECRET

```bash
PORT=80 WS_SECRET=[your secret] npm start
```

##Donations
MOAC: 0x53be4cb8f27152893b448f9f569624afd1a97e0c

