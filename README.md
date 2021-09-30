# Filecoin Fission Network Setup Instructions

Attention! This is all very pre alpha testing and might be unstable.

## Next planned reset

- 8th of October 2021 - UTC+8 morning

## Installation

The setup of a fission network node and miner follows the normal lotus setup steps. Please refer to the lotus docs:

Node setup: https://docs.filecoin.io/get-started/lotus/installation

Miner setup: https://docs.filecoin.io/mine/lotus/miner-setup

Instead of cloning and building the original lotus, clone and build:

`git clone https://github.com/Factor8Solutions/lotus`

`cd lotus`

`git checkout fission-ntwk`

`make clean fissionnet`

Follow the normal steps on how to run a node and/or a miner in the documentation.

When initializing the miner use:

`lotus-miner fetch-params 512MiB`

`lotus-miner init [.....] --sector-size 512MiB`

## Facts about Fission Network

The network is in a very early testing phase. There is no faucet and therefore it makes no sense to join for test mining without coordinating first. Please contact `Patrick - Factor8 Solutions` on the Filecoin Slack to get some FIL!

### Sector Size

- 512MiB only

### Min. required power for rewards

- 10GB

### Bottstrap core

- 2 miner with 50GB each running
- 2 nodes

### WaitSeed

- 10 minutes


## Fission Network planned timeline 

We hope to get a stable 512MiB testnet running by the end of the year! If you are interested in running a node or permanent miners please let us know.

### Now until November 1st - Non Public testing

- frequent resets expected
- no faucet
- network params might change
- no notary
- non public in the sense of not being able to get FIL for mining automatically - we nned to keep track of a few prams regarding mining participants and have o faucet yet

### November 2021 - Public Alpha testing 

- working faucet
- notary for verified deals (at least manual)

### December 2021 - Public Beta testing

- stable network params

### 1st of January 2022 

- stable non test test network live