sntpsend
========

Tiny SNTP client.

sntpsend behave as one-time SNTP client, but does not update system time.

License
-------

zlib License.

Target environments
-------------------

Windows, Cygwin, Linux, Mac OS X, FreeBSD.

sntpsend is Perl 5 script, and so probably works fine on other OS.

Set up
------

1. Install Perl 5.14 or later.
2. Put sntpsend in a directory registered in PATH.
3. (Windows only) Put sntpsend.bat in a directory registered in PATH.

Usage
-----

Please check help message `sntpsend --help`

Example
-------

```sh
# Test local NTP server (192.0.2.13:123)
sntpsend --host 192.0.2.13

# Test another local NTP server (192.0.2.14:8123)
sntpsend --host 192.0.2.14 --port 8123

# You can bind socket to UDP port 123 (see RFC 2030).
sntpsend --bind-sntp-port --host 192.0.2.13
```
