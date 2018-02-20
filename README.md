# Bitcoin Gold

[![Build Status](https://travis-ci.org/BTCGPU/BTCGPU.svg?branch=master)](https://travis-ci.org/BTCGPU/BTCGPU)

Bitcoin Gold (codename BTCGPU) is a fork of the Bitcoin blockchain that will occur at block height 491407, at roughly 12:00:00 UTC October 25, 2017.

At the predetermined block height, Bitcoin Gold miners will begin creating blocks with a new proof-of-work algorithm, and this will cause a bifurcation of the Bitcoin blockchain. The original Bitcoin blockchain will continue on unaltered, but a new branch of the blockchain will split off from the original chain. The new branch is a distinct blockchain with the same transaction history as Bitcoin up until the fork, but then diverges from it. As a result of this process, a new cryptocurrency will be born.


<<<<<<< HEAD
## Links
=======
sudo apt-get -y update<br>
sudo apt-get -y upgrade<br>

\# You may need to reboot your system after upgrade<br>

sudo apt-get install -y wget<br>
sudo apt-get install -y curl<br>
sudo apt-get install -y git<br>
sudo apt-get install -y build-essential<br>
sudo apt-get install -y autoconf<br>
sudo apt-get install -y automake<br>
sudo apt-get install -y libtool<br>
sudo apt-get install -y pkg-config<br>
sudo apt-get install -y libevent-dev<br>
sudo add-apt-repository ppa:bitcoin/bitcoin<br>
sudo apt-get update<br>
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev<br>
sudo apt-get install -y libboost-all-dev<br>
sudo apt-get install -y libssl-dev<br>
sudo apt-get install -y libzmq3-dev<br>
sudo apt-get install -y qdbus qmlscene qt5-default qt5-qmake qttools5-dev-tools qtbase5-dev-tools qtchooser qtdeclarative5-dev xbitmaps xterm libqt5svg5-dev qttools5-dev qtscript5-dev qtdeclarative5-folderlistmodel-plugin qtdeclarative5-controls-plugin<br>

**Install libsodium Using a Workaround**<br><br>
wget http://de.archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium-dev_1.0.13-1_amd64.deb<br>
wget http://de.archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium18_1.0.13-1_amd64.deb<br>
sudo dpkg -i libsodium*deb<br>
rm libsodium18_1.0.13-1_amd64.deb<br>
rm libsodium-dev_1.0.13-1_amd64.deb<br>

**Get Source Code from GitHub and Build**<br><br>
git clone https://github.com/gokhankocak/KadiCoin.git<br>
cd KadiCoin<br>
./autogen.sh<br>
./configure<br>
make<br>
sudo make install<br>

**Create Config File**<br><br>
mkdir ~/.KadiCoin<br>
cd ~/.KadiCoin<br>
nano KadiCoin.conf<br>

**Sample KadiCoin.conf**<br><br>
\# Online Config Generator:<br>
\# https://jlopp.github.io/bitcoin-core-config-generator/

server=1<br>
\# Bind to given address and always listen on it. Use [host]:port notation for IPv6. Replace it with your own IP.<br>
\# bind=192.168.0.26<br>

\# Specify a non-default location to store blockchain and other data.<br>
\# datadir=/data<br>

\# Run this node on the Bitcoin Test Network.<br>
\# testnet=1<br>

\# Run this node on its own independent test network.<br>
regtest=1<br>

\# Username for JSON-RPC connections<br>
rpcuser=kadicoinrpcuser<br>

\# Password for JSON-RPC connections<br>
rpcpassword=Put Some Strong Password Here<br>

**Run KadiCoind**<br><br>
\# Run KadiCoind and see its messages on your console<br>
KadiCoind -printtoconsole<br>
\# Run KadiCoind as a daemon (service)<br>
KadiCoind -daemon<br>

>>>>>>> 57e6e64b37aab13eb7c21aca6fb22dafec4e3dde

* Website: http://btcgpu.org
* Slack: [invitation](https://join.slack.com/t/bitcoin-gold/shared_invite/enQtMjY1MzkzMzUxNjY4LWM1YmQ4MjZhZTQxMWE1ZDQyNjA4N2QwZTkyZjYzMjhiMzdlMmVkNjQ3NzZlZDdmMDE4NWIyY2JmYzdjYmE2MzA)
* TODO-list: https://trello.com/b/P1rLw1G9/bitcoin-gold-todos
