Version 0.0.0.4
===============

An initial attempt at handling invalid commands has been added by
flushing the connection buffer each time a command or query is sent.

Queries now raise an `IOError` if they return the message `Fail` (it
could also be due to the previous command failing if the buffer
flush mentioned above did not catch the error).

Added the debugmcpi example. This is now built, along with hmcpi,
by setting the build-debug configure option (which is turned off
by default).

Version 0.0.0.3
===============

The examples - apart from `hmcpi` - now accept the `--debug` command-line
option which causes the messages sent to, and received from, MineCraft
to be printed to the standard-error channel. The format of these 
messages has been changed slightly.

Version 0.0.0.2
===============

Minor document improvements. Added examples/XJump.hs, which is the
example used in the documentation for Network.MineCraft.Pi.Client.

Version 0.0.0.1
===============

Initial version.
