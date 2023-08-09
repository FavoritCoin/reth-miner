# Reth-miner v0.0.2
## Our community
[Telegram pool](https://t.me/Altcoin_Pool)

[Telegram media](https://t.me/FavoritCoinChat)

[Discord](https://discord.gg/HqyjXaRX)

[Our pool](https://altcoinpool.ru)

## Donations
0x373C42955c4fC778b257BD1aCCF0b0349830a725

## Features
* NVIDIA CUDA mining v11.7.1 Only Nvidia
  
## Metamask Wallet settings

Name: Rethereum

RPC: https://rpc.rethereum.org/

Chain ID: 622277

Symbol: RTH

Explorer: https://explorer.rethereum.org/

## Installation in hive os

hive-replace -y --stable  (‼️hive will reset to the stable version ‼️)

disk-expand  (expand disk space)

apt update && apt upgrade

apt --only-upgrade install nvidia-settings xserver-xorg-core

do-release-upgrade   (the process is long, press Y everywhere, press enter on the purple screen)

miner stop

mkdir reth-miner && cd reth-miner

wget https://github.com/FavoritCoin/reth-miner/releases/download/v0.0.2/reth-miner.zip && unzip reth-miner.zip && rm -rf reth-miner.zip

sudo nano start.sh 

## Copy content between lines
------------------------------------------
#!/bin/bash 

./RTH_CUDA_GPU_Miner -P stratum://0x1cDD22aad741fe62519914370284Ac3E401b5218@ru-stratum.altcoinpool.ru:4054 (at the end of the wallet are symbols    @ru)
------------------------------------------

sudo chmod +x ./start.sh && sudo chmod +x ./RTH_CUDA_GPU_Miner

screen -S rth (any name I have rth)

./start.sh

## If you have restarted the farm and want to restart mining, enter alternately:

cd reth-miner
screen -S rth
./start.sh

## If HiveShell is closed, but you really want to see the mining process, then open HiveShell again and enter one by one:

cd reth-miner
screen -r rth


### More information

For more information about building or command line usage and other options please checkout the [Ethminer](https://github.com/ethereum-mining/ethminer) project.

## Credits

| Name                  | Contact                                                      |     |
| --------------------- | ------------------------------------------------------------ | --- |
| ETHMiner Team    | [Ethminer](https://github.com/ethereum-mining/ethminer)     |  |
| Blake3 Team                   | [Blake3](https://github.com/BLAKE3-team/BLAKE3)                               |     |
| Gellin                | [@Gellin](https://github.com/gellin)                         |  RTH - 0xF5d15ae0c0E0e2da707266FdFcC5772a0583A417   |
| k1                | [@k1](https://github.com/korbin)                         |    |
| AllFather |  |    |

## Contribute

To meet the community, ask general questions and chat about ethminer join us on [discord](https://discord.gg/kBSnzqyph2).

All bug reports, pull requests and code reviews are very much welcome.


## License

Licensed under the [GNU General Public License, Version 3](LICENSE).
