
To RUN the project use below commands


1. Install NPM
npm install

2. Start the server
gulp serve


Potential Errors:
"Cannot find where you keep your Bower packages"
> Solution:  Install bower. 
	npm i -g bower
	bower install




--------------------------------------------------------------------------------

TO START PRIVATE-net, please use the below commands

WINDOWS:
=======

Create a data folder and initialize the genesis data via this command: 

geth.exe --datadir=./data init C:\Training\Blockchain-Course-Geth\genesis.json


Set the rpc information, specifically the cors domain, the api protocols, and the ports:

geth.exe --datadir=./data --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "127.0.0.1" --rpcport "8545"

Attach to the network via command line

Geth\geth.exe attach

Run this comand once attached to the network:

"Ethereum-Wallet\Ethereum Wallet.exe" --node-datadir=./data



UBUNTU:
=======

Create a data folder and initialize the genesis data via this command: 

./build/bin/geth --datadir=./data/test init genesis/genesis.json

Set the rpc information, specifically the cors domain, the api protocols, and the ports:

./build/bin/geth  --datadir=./data/test --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "localhost" --rpcport "8545"

Attach to the network via command line

#./build/bin/geth attach --datadir=./data/test

./build/bin/geth attach http://localhost:8545

Run this comand once attached to the network:

/home/<<username>>/Installed/mist/mist --rpc=http://localhost:8545

/home/<<username>>/Installed/ethereum-wallet/ethereumwallet --rpc=http://localhost:8545


MAC:
===

Create a data folder and initialize the genesis data via this command: 

geth --datadir=./data init genesis.json

Set the rpc information, specifically the cors domain, the api protocols, and the ports:

geth --datadir=./data --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "127.0.0.1" --rpcport "8545"

Attach to the network via command line

geth attach http://127.0.0.1:8545

Run this comand once attached to the network:

open -a /Applications/Mist.app —args —node-datadir=./data (Mist Waller)


=============================================

INSTALLING SOLIDITY AND TRUFFLE

OFFICIAL DOCS-
	Solidity: http://solidity.readthedocs.io/en/develop/installing-solidity.html
	Truffle: http://truffleframework.com/docs/getting_started/installation

STEP BY STEP SOLIDITY- 

npm install -g solc

MAC OS- sudo xcodebuild -license accept

STEP BY STEP TRUFFLE-
1. npm install -g truffle
1A_for windows, if you face a naming conflict, please use - http://truffleframework.com/docs/advanced/configuration#resolving-naming-conflicts-on-windows

To test truffle, create a new folder and try:
truffle init 


