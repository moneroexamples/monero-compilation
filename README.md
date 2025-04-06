# monero-compilation

Basic instruction on compliation of monero v0.18 (monero branch `release-v0.18`) 
for use in moneroexamples projects.

## Example compilation of Monero on Ubuntu 24.04

```bash
# first install monero dependecines
sudo apt update

sudo apt install git build-essential cmake libboost-all-dev miniupnpc libunbound-dev graphviz doxygen libunwind8-dev pkg-config libssl-dev libcurl4-openssl-dev libgtest-dev libreadline-dev libzmq3-dev libsodium-dev libhidapi-dev libhidapi-libusb0

# go to home folder
cd ~
git clone --recursive -b release-v0.18 https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


## Example compilation of master branch (i.e., development version of Monero) on Ubuntu 22.04

```bash
# first install monero dependecines
sudo apt update

sudo apt install git build-essential cmake libboost-all-dev miniupnpc libunbound-dev graphviz doxygen libunwind8-dev pkg-config libssl-dev libcurl4-openssl-dev libgtest-dev libreadline-dev libzmq3-dev libsodium-dev libhidapi-dev libhidapi-libusb0

# go to home folder
cd ~
git clone --recursive https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


## Example compilation of master branch (i.e., development version of Monero) on Arch

```bash
sudo pacman -Syu git base-devel boost cmake miniupnpc unbound libunwind openssl hidapi zeromq readline xz graphviz libsodium gtest

# go to home folder
cd ~

git clone --recurse-submodules https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


## Example compilation on Fedora 35

```bash
sudo dnf install git gcc-c++ cmake boost-devel pkgconf openssl-devel cppzmq-devel unbound-devel libsodium-devel libunwind-devel xz-devel hidapi-devel make libatomic curlpp-devel miniupnpc readline-devel

# go to home folder
cd ~

git clone --recurse-submodules  -b release-v0.18 https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


