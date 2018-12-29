EblockmailCoin (fork of PIVX) integration/staging repository
======================================


It is recommended [use the shell script](https://github.com/eblockmail/birinstall) to install a EblockmailCoin Masternode on a Linux server running Ubuntu 14.04 or 16.04

***

Quick installation of the EblockmailCoin daemon under linux. See detailed instructions there [build-unix.md](https://github.com/eblockmail/ebm/blob/master/doc/build-unix.md)

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/eblockmail/ebm.git
    cd ebm
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip ebmd
    sudo strip ebm-cli
    sudo strip ebm-tx
    cd ..

Running the daemon:

    ebmd 

Stopping the daemon:

    ebm-cli stop

Demon status:

    ebm-cli getinfo
    ebm-cli mnsync status

All binaries for different operating systems, you can download in the releases repository:

https://github.com/eblockmail/ebm/releases

P2P port: 3434, RPC port: 3435
-
Distributed under the MIT software license, see the accompanying file COPYING or http://www.opensource.org/licenses/mit-license.php.
