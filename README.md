# MVPN

-------------------------
 Secure IP tunnel daemon
-------------------------

:Manual section: 8
:Manual group: System Manager's Manual



SYNOPSIS
========
| ``mvpn`` [ options ... ]
| ``mvpn``  ``--help``



INTRODUCTION
============

MVPN is an open source VPN daemon by James Yonan. Because MVPN
tries to be a universal VPN tool offering a great deal of flexibility,
there are a lot of options on this manual page. If you're new to
MVPN, you might want to skip ahead to the examples section where you
will see how to construct simple VPNs on the command line without even
needing a configuration file.


And if you would like to see a shorter version of this manual, see the
MVPN usage message which can be obtained by running **MVPN**
without any parameters.



DESCRIPTION
===========

MVPN is a robust and highly flexible VPN daemon. MVPN supports
SSL/TLS security, ethernet bridging, TCP or UDP tunnel transport through
proxies or NAT, support for dynamic IP addresses and DHCP, scalability
to hundreds or thousands of users, and portability to most major OS
platforms.

MVPN is tightly bound to the OpenSSL library, and derives much of its
crypto capabilities from it.

MVPN supports conventional encryption using a pre-shared secret key
**(Static Key mode)** or public key security **(SSL/TLS mode)** using
client & server certificates. MVPN also supports non-encrypted
TCP/UDP tunnels.

MVPN is designed to work with the **TUN/TAP** virtual networking
interface that exists on most platforms.

Overall, MVPN aims to offer many of the key features of IPSec but
with a relatively lightweight footprint.



OPTIONS
=======

MVPN allows any option to be placed either on the command line or in
a configuration file. Though all command line options are preceded by a
double-leading-dash ("--"), this prefix can be removed when an option is
placed in a configuration file.

.. include:: man-sections/generic-options.rst
.. include:: man-sections/log-options.rst
.. include:: man-sections/protocol-options.rst
.. include:: man-sections/client-options.rst
.. include:: man-sections/server-options.rst
.. include:: man-sections/encryption-options.rst
.. include:: man-sections/cipher-negotiation.rst
.. include:: man-sections/network-config.rst
.. include:: man-sections/script-options.rst
.. include:: man-sections/management-options.rst
.. include:: man-sections/plugin-options.rst
.. include:: man-sections/windows-options.rst
.. include:: man-sections/advanced-options.rst
.. include:: man-sections/unsupported-options.rst
.. include:: man-sections/connection-profiles.rst
.. include:: man-sections/inline-files.rst
.. include:: man-sections/signals.rst
.. include:: man-sections/examples.rst


FAQ
===





HOWTO
=====

For a more comprehensive guide to setting up MVPN in a production
setting, see the MVPN HOWTO at




PROTOCOL
========

For a description of MVPN's underlying protocol, see




WEB
===


Go here to download the latest version of MVPN, subscribe to the
mailing lists, read the mailing list archives, or browse the SVN
repository.



BUGS
====

Report all bugs to the MVPN team 



SEE ALSO
========

``dhcpcd``\(8),
``ifconfig``\(8),
``openssl``\(1),
``route``\(8),
``scp``\(1)
``ssh``\(1)



NOTES
=====

This product includes software developed by the OpenSSL Project
(https://www.openssl.org/)

For more information on the TLS protocol, see
http://www.ietf.org/rfc/rfc2246.txt

For more information on the LZO real-time compression library see
https://www.oberhumer.com/opensource/lzo/



COPYRIGHT
=========

Copyright (C) 2002-2020 MVPN Inc This program is free software; you
can redistribute it and/or modify it under the terms of the GNU General
Public License version 2 as published by the Free Software Foundation.

