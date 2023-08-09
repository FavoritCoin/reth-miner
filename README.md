# Reth-miner v0.0.2

## Features
* NVIDIA CUDA mining v11.7.1 Только зелёные карты
  
## Metamask Wallet settings
Name: Rethereum
RPC: https://rpc.rethereum.org/
Chain ID: 622277
Symbol: RTH
Explorer: https://explorer.rethereum.org/

## installation in hive os

hive-replace -y --stable  (‼️hive сбросится до стабильной версии‼️)

disk-expand  (расширит дисковое пространство)

apt update && apt upgrade

apt --only-upgrade install nvidia-settings xserver-xorg-core

do-release-upgrade   (процесс долгий, везде нажимать Y, на фиолетовом экране нажать enter)

miner stop

mkdir reth-miner && cd reth-miner

wget https://github.com/Rethereum-blockchain/rethminer/releases/download/v0.0.2/rethminer.zip && unzip rethminer.zip && rm -rf rethminer.zip

sudo nano start.sh 

// Копировать содержимое между линиями
------------------------------------------
#!/bin/bash 

./RTH_CUDA_GPU_Miner -P stratum://0x66661.......d32bD12a20bC@ru-stratum.altcoinpool.ru:4054 (в конце кошелька символы    @ru)
------------------------------------------

sudo chmod +x ./start.sh && sudo chmod +x ./RTH_CUDA_GPU_Miner

screen -S rth (любое название у меня rth)

./start.sh

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

To meet the community, ask general questions and chat about ethminer join us on [discord](https://discord.com/invite/xCB4AJDEFb).

All bug reports, pull requests and code reviews are very much welcome.

## License

Licensed under the [GNU General Public License, Version 3](LICENSE).
