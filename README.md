Monero-Miner for Single board computers like Raspberry Pi, powered by [balena](https://balena.io)

![](https://raw.githubusercontent.com/iayanpahwa/monero-miner/master/assets/logo.png)

## Introduction
Support Monero blockchain, validating the transactions by lending your compute power from SBCs like a Raspberry Pi and earn XMRs (cryptocurrency of Monero blockchain) in return.

--------------------
## Hardware required

- A Raspberry Pi 4 (the more RAM it has the better) -- currently tested to work
- 16GB Micro-SD Card (recommended Sandisk Extreme Pro SD cards)
- Power supply for the Pi

--------------------
## Software required

- Monero Wallet to receive the XMR rewards, download from [here](http://getmonero.org/downloads/#gui)

--------------------
## Deploy a fleet

You can deploy this app to a new balenaCloud fleet in one click using the button below:

[![deploy button](https://balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/iayanpahwa/monero-miner)


Or, you can create a fleet in your balenaCloud dashboard, clone this repo and `balena push` this code to it, the traditional way.

--------------------

#### Configuring the miner

The following [Device Configuration](https://www.balena.io/docs/learn/manage/configuration/#configuration-variables) variables are required, these can be set at balenaCloud dashboard :


| Name                                  | Value                                                                                     |
| ------------------------------------- | ----------------------------------------------------------------------------------------- |
| WALLET_ADDRESS                        | Change this to your monero wallet address which you install and set
| MINER_POOL                            | (Optional) Change this to the mining pool you want to join, default is: ```xmr.2miners.com:2222```                           |

--------------------

Attribution

- [XMRig project](https://github.com/xmrig)