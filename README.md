# GGCash-Core
# Version: 1.0.0.0
Official GGCash Core Cryptocurrency Repository.

# Contact:
> 💬Telegram:
**https://t.me/GGcash**

> 💬Facebook:
**...**

> 💬Twitter:
**...**

> 💬BTCTalk:
**...**

> ✉️E-mail:
**contato@ggcash.online**

> 🌎Website:
**https://ggcash.online**

> 🌎Block Explorer:
**https://explorer.ggcash.online**

# ESPECIFICAÇÕES:
- **Nome:** GGCash <br>
- **Simbolo:** GGH <br>
- **Algoritimo:** Quark <br>
- **Block type:** PoS/PoW/MN <br>
- **Reward	(PoW):** 2.24 GGH's - end time block: 35.000 <br>
- **Reward (PoS):** 2.24 GGH's <br>
- **Reward Superblock:** 3% <br>
- **Reward Masternode:** 72% <br>
- **Masternode amount:** 30000 GGH's <br>
- **Confirmações de Masternode:** 21 blocos <br>
- **Maturidade de Masternode:** 20 <br>
- **BlockTime:** 3 minutes <br>
- **Resete Dificuldade:**	3 minutes <br>
- **Confirmações de Transação:** 5 blocos <br>

**Use the following instructions to compile a daemon and GUI wallet for Ubuntu Server 18.04.**

**Update your Ubuntu machine.**

sudo apt-get update<br>
sudo apt-get upgrade<br>

**Install the required dependencies.**

sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl1.0-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev libboost-all-dev libboost-program-options-dev -y<br>

sudo apt-get install libminiupnpc-dev libzmq3-dev libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler libqrencode-dev unzip libgmp3-dev -y<br>

**Install Berkeley DB.**

sudo add-apt-repository ppa:bitcoin/bitcoin<br>
sudo apt-get update<br>
sudo apt-get install libdb4.8-dev libdb4.8++-dev -y<br>

**Create a directory for the source code.**

cd ~/<br>
mkdir source_code<br>

**Download the source code from Github.**

sudo apt-get install git -y<br>
git clone https://github.com/GGCash/GGCash-Core.git source_code<br>
cd source_code<br>
./autogen.sh<br>
./configure --with-incompatible-bdb<br>
make<br>

**the ggcashd ggcash-cli and ggcash-tx files are in source_code/src**<br>

**the ggcash-qt file will be in source_code/src/qt**<br>

**move files to usr/bin**<br>

# ggcash.conf
```sh
rpcuser=rpc_exampleuser
rpcpassword=exemplepass
rpcallowip=0.0.0.0/0
listen=1
server=1
txindex=1
daemon=1
addnode=5.189.151.31
addnode=207.180.225.42
```
