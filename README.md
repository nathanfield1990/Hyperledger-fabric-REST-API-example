# Hyperledger-fabric-REST-API-example

Instructions
- Install the latest binaries https://hyperledger-fabric.readthedocs.io/en/latest/install.html
- Run through test network https://hyperledger-fabric.readthedocs.io/en/release-2.4/test_network.html

- Instructions after installing fabric-samples and running test network

Good reference article https://kctheservant.medium.com/deep-dive-into-fabcar-revised-57cb54642572

Copy javascript folder in fabcar and call it apiserver (in same location as it)

Create a new file called apiserver.js in apiserver folder, copy / paste from here https://github.com/thomastibin/apiserver/blob/master/apiserver/apiserver.js

Cd into apiserver folder and run npm install express body-parser --save

cd ..   (into fabcar)

./startFabric.sh javascript

cd apiserver

node enrollAdmin.js 

node registerUser.js

**If above two don't work, delete wallet contents in apiserver location**

sudo npm install -g nodemon (if needed to install dependencies)

nodemon apiserver.js

You can now issue REST instructions to the active server, Node-RED was used 

===============================================================

Node-RED, att HTTP request nodes
GET to http://Server_IP_Address:8080/api/queryallcars
POST to http://Server_IP_Address:8080/api/addcar

