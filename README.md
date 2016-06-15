# Asterisk PBX - GoTrunk reference configuration

This repository contains complete set of configuration files for Asterisk PBX to be used with GoTrunk SIP Trunking service.

There are two branches:

* [static-ip](https://github.com/GoTrunk/asterisk-config/tree/static-ip) - to be used with Asterisk on Static IP address
* [dynamic-ip](https://github.com/GoTrunk/asterisk-config/tree/dynamic-ip) - to be used with Asterisk on Dynamic IP address

This configuration files has been tested with Asterisk 11 and Asterisk 13.


## Usage instructions

### Install Asterisk

#### Debian

Install required packages:
```
apt-get install build-essential openssl libxml2-dev libncurses5-dev uuid-dev sqlite3 libsqlite3-dev pkg-config libjansson-dev
```

Get Asterisk source, compile and install:

Asterisk 11
```
cd /usr/src
wget http://downloads.asterisk.org/pub/telephony/asterisk/asterisk-11-current.tar.gz
tar xf asterisk-11-current.tar.gz
cd asterisk-*
./configure
make && make install
```

Asterisk 13
```
cd /usr/src
wget http://downloads.asterisk.org/pub/telephony/asterisk/asterisk-13-current.tar.gz
tar xf asterisk-13-current.tar.gz
cd asterisk-*
./configure
make && make install
```
