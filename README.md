mifo (1.5)
---------

MPlayer daemon with preset/native commands controlled through a FIFO
Written in ZSH

---------

Requirements:

ZSH + MPLAYER + PROCPS(ps|pgrep|pkill) + COREUTILS(mkfifo)

---------

Todo:

Looking to remove PROCPS and COREUTILS dependencies but may not..

---------

Currently in developmental stage.. if you experience any problems PLEASE contact me.

---------

Added systemd service script.
Recommended starting under user-session@..
  % systemd --user start mifo
  % systemd --user stop mifo

or simply..

  % mifo --init
  % mifo --quit
