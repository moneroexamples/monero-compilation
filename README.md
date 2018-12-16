# monero-compilation

Basic instruction on compliation of monero for use in moneroexamples projects.

## Example compilation on Ubuntu 18.04

```bash
# first install monero dependecines
sudo apt update

sudo apt install git build-essential cmake libboost-all-dev miniupnpc libunbound-dev graphviz doxygen libunwind8-dev pkg-config libssl-dev libcurl4-openssl-dev libgtest-dev libreadline-dev libzmq3-dev libsodium-dev libhidapi-dev libhidapi-libusb0

# go to home folder
cd ~

git clone --recurse-submodules https://github.com/monero-project/monero

cd monero/

USE_SINGLE_BUILDDIR=1 make
```




