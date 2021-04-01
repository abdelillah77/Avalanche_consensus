# Avalanche

Avalanche is a layer one protocol by Ava Labs that offers high-throughput, fast finality, and unprecedented decentralization. Developers are able to launch their own public or private blockchains (called subnets), create and trade digital assets, and build scalable smart contracts and decentralized applications.
Subnets within the Avalanche network will be highly customizable and will have their own incentive structures.
Because of this customization, companies can create legally compliant permissioned subnets while still being connected to the grander Avalanche network. This could lead to the creation of new financial primitives and bring more traditional financial products into the blockchain space in a decentralized way.

Implementation of the Avalanche consensus protocol. Avalanche is a performant, leaderless, secure consensus protocol.

## Setup & Installation

The use of virtualenv is needed to run the project. The project uses Python3.6+.

```
virtualenv -p python3.6 venv
```

Then, install the dependencies

```
pip install -r requirements.txt
```

## Running the testnet

The `src/testnet.sh` script will spawns a Redis server and local processes that will interact with each other in a peer-to-peer fashion.

These nodes will randomly generate transactions to fill up the blockchain.

```
cd src
./testnet.sh

# add MAX_NODES to increase the number of nodes in the local network
MAX_NODES=15 ./testnet.sh
```

## Running tests

From the root directory, run the command:

```
python -m pytest tests
```
