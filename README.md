# electrumx-installer

Electrumx installation script.

Installing electrumx isn't really straight-forward (yet). You have to install the latest version of Python and various dependencies for one of the database engines. Then you have to integrate electrumx into your init system.

`electrumx-installer` simplifies this process to running a single command. All that's left to do for you
is to customise the configuration and to start electrumx.

## Usage

This installs electrumx using the default options:

	wget https://raw.githubusercontent.com/cyberyen-squat/electrumx-installer/master/bootstrap.sh -O - | bash

You can also set some options if you want more control:

| -d --dbdir | Set database directory (default: /db/) |
|------------|----------------------------------------|
| --update   | Update previously installed version    |
| --leveldb  | Use LevelDB instead of RocksDB         |

For example:

	wget https://raw.githubusercontent.com/cyberyen-squat/electrumx-installer/master/bootstrap.sh -O - | bash -s - -d /media/ssd/electrum-db


## Operating System Compatibility

The following operating systems are officially supported and automatically being tested against:

| OS             |
|----------------|
| Ubuntu 20.04   |
| Ubuntu 18.04   |
| Ubuntu 16.04   |
| Fedora 29      |
| CentOS 7       |
| Debian Stretch |
| Debian Buster  |


If you prefer a different operating system that's not listed here, see
[`distributions/README.md`](https://github.com/cyberyen-squat/electrumx-installer/blob/master/distributions/README.md) to find out how to add it.
Or open an [issue](https://github.com/cyberyen-squat/electrumx-installer/issues/new) if you'd rather not do that yourself.


### Ask for help

Here is the place to contact us:
[c¥talk [Matrix]](https://matrix.to/#/#cykuza-cytalk:matrix.org)
