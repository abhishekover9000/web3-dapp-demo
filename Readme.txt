
To RUN the project use below commands


1. Install NPM
npm install

2. Start the server
gulp serv


--------------------------------------------------------------------------------

TO START PRIVATE-net, please use the below commands



WINDOWS:
=======

geth.exe --datadir=./data init C:\Training\Blockchain-Course-Geth\genesis.json

geth.exe --datadir=./data --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "127.0.0.1" --rpcport "8545"

Geth\geth.exe attach

Ethereum-Wallet\Ethereum Wallet.exe" --node-datadir=./data



UBUNTU:
=======

./build/bin/geth --datadir=./data/test init genesis/genesis.json

./build/bin/geth  --datadir=./data/test --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "localhost" --rpcport "8545"

#./build/bin/geth attach --datadir=./data/test

./build/bin/geth attach http://localhost:8545

/home/<<username>>/Installed/mist/mist --rpc=http://localhost:8545

/home/<<username>>/Installed/ethereum-wallet/ethereumwallet --rpc=http://localhost:8545


MAC:
===

geth --datadir=./data --rpc --rpccorsdomain "http://localhost:8000" --rpcapi "db,eth,net,web3,personal,miner"  --rpcaddr "127.0.0.1" --rpcport "8545
geth attach http://127.0.0.1:8545

open -a /Applications/Mist.app —args —node-datadir=./data (Mist Waller)