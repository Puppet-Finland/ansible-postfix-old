# ansible-postfix

An ansible role that install and configures postfix, and optionally monitors it 
with monit. Right now this module assumes that emails go through through a 
relayhost that requires authentication (i.e. sasl_passwd is configured by 
default).

# Operating system support

This module has been tested on

* Ubuntu 16.04

It has built-in support for Debian, RedHat and FreeBSD, but those are not 
guaranteed to work right now. In practice non-systemd distros are not yet 
supported, though adding support would be fairly trivial by just adding a 
service-manager -specific variable file.
