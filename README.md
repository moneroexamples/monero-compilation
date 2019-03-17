# monero-compilation

Basic instruction on compliation of monero v0.14.0.2 (monero branch `release-v0.13`) 
for use in moneroexamples projects.

## Example compilation on Ubuntu 18.04

```bash
# first install monero dependecines
sudo apt update

sudo apt install git build-essential cmake libboost-all-dev miniupnpc libunbound-dev graphviz doxygen libunwind8-dev pkg-config libssl-dev libcurl4-openssl-dev libgtest-dev libreadline-dev libzmq3-dev libsodium-dev libhidapi-dev libhidapi-libusb0

# go to home folder
cd ~
git clone --recursive -b release-v0.13 https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```

## Example compilation on Arch

```bash
sudo pacman -Syu git base-devel boost cmake miniupnpc unbound libunwind openssl hidapi zeromq readline xz graphviz libsodium

# go to home folder
cd ~

git clone --recursive -b release-v0.13 https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


## Example compilation on Fedora 29

```bash
sudo dnf install git gcc-c++ cmake boost-devel pkgconf openssl-devel cppzmq-devel unbound-devel libsodium-devel libunwind-devel xz-devel hidapi-devel

# go to home folder
cd ~

git clone --recursive -b release-v0.13 https://github.com/monero-project/monero.git

cd monero/

USE_SINGLE_BUILDDIR=1 make
```


