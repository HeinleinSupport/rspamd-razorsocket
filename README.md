# rspamd-razorsocket

Small Perl Daemon to use Razor2 over TCP Sockets. Mainly to use Razor2 with Rspamd.

## Razor2

[http://razor.sourceforge.net/](http://razor.sourceforge.net)

Vipul's Razor is a distributed, collaborative, spam detection and filtering network. Through user contribution, Razor establishes a distributed and constantly updating catalogue of spam in propagation that is consulted by email clients to filter out known spam. Detection is done with statistical and randomized signatures that efficiently spot mutating spam content. User input is validated through reputation assignments based on consensus on report and revoke assertions which in turn is used for computing confidence values associated with individual signatures.

# Installation

## Install Razor2

-   use cpan, apt, yum, zypper or the source to install the razor2 agent on your system

## Install Razorsocket

-   edit razorsocket config section to fit your needs
-   copy razorsocket daemon file to /usr/local/bin
-   copy the systemd service file razorsocket.service to /etc/systemd/system
-   enable and unmask the Service
~~~
systemctl unmask razorsocket.service
systemctl enable razorsocket.service
~~~

## Firewall settings for Razor2

-   Port 2703 / TCP
-   Port 7 / TCP

# License

Apache-2.0

# Author Information

~~~
Heinlein Support GmbH
Schwedter Str. 8/9b, 10119 Berlin

https://www.heinlein-support.de

Tel: 030 / 405051-10

Amtsgericht Berlin-Charlottenburg - HRB 93818 B
Geschäftsführer: Peer Heinlein - Sitz: Berlin
~~~
