# Hyperledger-fabric-REST-API-example

Instructions
- Install the latest binaries https://hyperledger-fabric.readthedocs.io/en/latest/install.html
- Run through test network https://hyperledger-fabric.readthedocs.io/en/release-2.4/test_network.html

- Instructions after installing fabric-samples and running test network
Create a new file called apiserver.js in apiserver folder, copy / paste from here https://github.com/thomastibin/apiserver/blob/master/apiserver/apiserver.js
Run node-red – exported flow 

Copy javascript folder in fabcar and call it apiserver

Cd into it and run npm install express body-parser --save

cd ..

./startFabric.sh javascript

cd apiserver

node enrollAdmin.js

node registerUser.js

sudo npm install -g nodemon (if needed)

nodemon apiserver.js


