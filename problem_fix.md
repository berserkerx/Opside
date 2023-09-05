# SYNC konusunda sorun yaşadıysan V2 Fix:

> Bir kaç neden var burada, mnemonicleri eksik girmek veya genesisi indirmemek.

> Rehberimden yapıldıysa sorun yok, önceden kurmaya calısan arkadaşlar için çözüm:

```sh
# Genesisi yükleyelim
cd
cd testnet-auto-install-v2
wget -c https://pre-alpha-download.opside.network/testnet-auto-install.tar.gz 
tar -C ./ -xzf testnet-auto-install.tar.gz
chmod +x -R ./testnet-auto-install
cd ./testnet-auto-install
```
```sh
# Tüm sistemleri durduralım:
opside-chain/stop-all.sh
```
```sh
# Tekrar başlatalım
cd
testnet-auto-install-v2/opside-chain/start-geth.sh
testnet-auto-install-v2/opside-chain/start-beaconChain.sh
testnet-auto-install-v2/opside-chain/start-validator.sh
```
```sh
cd testnet-auto-install-v2/
cd testnet-auto-install

# Loglara bakabirsiniz nodunuz temiz bir şekilde çalışacak.
opside-chain/show-geth-log.sh

opside-chain/show-beaconChain-log.sh

opside-chain/show-validator-log.sh
```
# SYNC konusunda sorun yaşadıysan V3 Fix:
```
# Genesisi yükleyelim
cd
wget -c https://pre-alpha-download.opside.network/testnet-auto-install-v3.tar.gz
tar -C ./ -xzf testnet-auto-install-v3.tar.gz
chmod +x -R ./testnet-auto-install-v3
cd ./testnet-auto-install-v3
```
```sh
# Tüm sistemleri durduralım:
opside-chain/stop-all.sh
```
```sh
# Tekrar başlatalım
cd
testnet-auto-install-v3/opside-chain/start-geth.sh
testnet-auto-install-v3/opside-chain/start-beaconChain.sh
testnet-auto-install-v3/opside-chain/start-validator.sh
```
```sh
cd testnet-auto-install-v3/
# Loglara bakabirsiniz nodunuz temiz bir şekilde çalışacak.
opside-chain/show-geth-log.sh
opside-chain/show-beaconChain-log.sh
opside-chain/show-validator-log.sh
