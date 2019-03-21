Dash Black Core integration/staging repository
=================================================

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev


Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/dashblackcoin/dashblack.git
    cd dashblack
    ./autogen.sh
    ./configure
    make
    make install


Running the daemon:

    dashblackd 

Stopping the daemon:

    dashblack-cli stop

Demon status:

    dashblack-cli getinfo
    dashblack-cli mnsync status


P2P port: 9748, RPC port: 9747
-
Distributed under the MIT software license, see the accompanying file COPYING or http://www.opensource.org/licenses/mit-license.php.
