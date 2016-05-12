# keter-debian

This is a script to install [Keter] on [Debian Jessie] (Debian 8.*). The
[script] provided in the Keter repository works on Ubuntu 14.04, but not
on Debian, or (I believe) any versions of Ubuntu that use systemd.

There are some small but subtle differences between the two
distributions. The most important difference is that Debian uses systemd
as its init system, and therefore, the Upstart script provided in the
normal keter repository does not work on Debian 8.* or greater.

## Usage

To run the script, run

    wget -O - https://raw.github.com/pharpend/keter-debian/master/setup-keter.sh | bash -ex

## Contact

The original author of this script is Michael Snoyman. If you have an
issue with Keter, you can open an issue in the
[keter repository][keter]. If you have any questions/concerns about this
script, you can either open up a GitHub issue, or email
`peter@harpending.org`.

[Debian]: https://www.debian.org/
[keter]: https://github.com/snoyberg/keter
[script]: https://github.com/snoyberg/keter/blob/master/setup-keter.sh
