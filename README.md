# KadiCoin

**KadiCoin**, yet another cryptocurrency. **KadiCoin** was born in **Kadikoy, Turkiye** where a group of friends meet at Kadikoy. This is an experimental project and I hope it will be a good beginning in our research and development activity.

# Installation

Operating System:
[Ubuntu Server 16.04.3 LTS](https://www.ubuntu.com/download/server)

**Install Prerequisities**

sudo apt-get -y update

sudo apt-get -y upgrade

\# You may need to reboot your system after upgrade

sudo apt-get install -y wget 
sudo apt-get install -y curl
sudo apt-get install -y git
sudo apt-get install -y build-essential
sudo apt-get install -y autoconf
sudo apt-get install -y automake
sudo apt-get install -y libtool
sudo apt-get install -y pkg-config
sudo apt-get install -y libevent-dev
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev
sudo apt-get install -y libboost-all-dev
sudo apt-get install -y libssl-dev
sudo apt-get install -y libzmq3-dev
sudo apt-get install -y qdbus qmlscene qt5-default qt5-qmake qttools5-dev-tools qtbase5-dev-tools qtchooser qtdeclarative5-dev xbitmaps xterm libqt5svg5-dev qttools5-dev qtscript5-dev qtdeclarative5-folderlistmodel-plugin qtdeclarative5-controls-plugin

**Install libsodium Using a Workaround**
wget http://de.archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium-dev_1.0.13-1_amd64.deb
wget http://de.archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium18_1.0.13-1_amd64.deb
sudo dpkg -i libsodium*deb
rm libsodium18_1.0.13-1_amd64.deb
rm libsodium-dev_1.0.13-1_amd64.deb

**Get Source Code from GitHub and Build**
git clone https://github.com/gokhankocak/KadiCoin.git
cd KadiCoin
./autogen.sh
./configure
make
sudo make install

**Create Config File**
mkdir ~/.KadiCoin
cd ~/.KadiCoin
nano KadiCoin.conf

**Sample KadiCoin.conf**
\# Online Config Generator:
\# https://jlopp.github.io/bitcoin-core-config-generator/

server=1
\# Bind to given address and always listen on it. Use [host]:port notation for IPv6. Replace it with your own IP.
\# bind=192.168.0.26

\# Specify a non-default location to store blockchain and other data.
\# datadir=/data

\# Run this node on the Bitcoin Test Network.
testnet=1

\# Run this node on its own independent test network.
\# regtest=1

\# Username for JSON-RPC connections
rpcuser=kadicoinrpcuser

\# Password for JSON-RPC connections
rpcpassword=PgJBtsFHuZ383n8.kp3M7g

**Run KadiCoind**
KadiCoind -printtoconsole
