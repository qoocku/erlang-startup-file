'.erlang' Startup File Which I have Just Invented With a Little Help of Google Search
-----------------------------------------------------------------------------------

This sweet startup file does the following:

1. Runs `toolbar` tool (a GUI with fancy tools like process monitor and others)
   under the name of "toolbar@127.0.0.1".
2. Sets the just started node name (if not set already) to be something like `$USER<n>` where `<n>`
   is choosen from the range of 1 to 256 -- it depends on what similar nodes
   has been started already. If the environment variable 'USER' is not set, than
   it reads 'HOME' variable stripping off everything but the last "home" directory
   name which is used as the node name prefix.
3. Connects the brand new named node to the "toolbar" node.

Note that in order to do (1) the "epmd" must be also started which this script does
automagically for me. Sweet.

Enjoy.

