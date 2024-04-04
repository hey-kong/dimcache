# Dimcache

## Dependencies

* libevent - https://www.monkey.org/~provos/libevent/ (libevent-dev)
* libseccomp (optional, experimental, linux) - enables process restrictions for
  better security. Tested only on x86-64 architectures.
* openssl (optional) - enables TLS support. need relatively up to date
  version. pkg-config is needed to find openssl dependencies (such as -lz).

## Build

To build dimcache in your machine from local repo you will have to install autotools, automake and libevent. In a Ubuntu based system that will look like this

```
sudo apt-get install pkg-config
sudo apt-get install autotools-dev
sudo apt-get install automake
sudo apt-get install libevent-dev
```

Then build dimcache

```
./autogen.sh
./configure
make
make test
```
