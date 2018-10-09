#!/bin/bash
apt-get upgrade -y 
apt-get update -y
apt-get install -y libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev git screen
git clone http://github.com/Supichai-ss/nimiq-beeppool
cd nimiq-beeppool
chmod +x miner
./miner --wallet-address='NQ22 QR5L 6BB5 5G70 6RQ2 DLLQ 968K H8B4 MH7V' --deviceLabel=LK03-EC2