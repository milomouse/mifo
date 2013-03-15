mifo (2.4)
---------

About:

* MPlayer daemon with preset/native commands controlled through a FIFO.

* Written in ZSH.

---------

Requirements:

* ZSH

* MPLAYER

* PROCPS (ps|pgrep|pkill)

* COREUTILS (mkfifo)

---------

Todo:

* Trying to remove PROCPS and COREUTILS dependencies but may not; will look into it..

* Currently unaware of native Zsh handling for external process collection.

* Currently unaware of native Zsh handling for fifo creation.

---------

Notes:

* Script is in its developmental stages although appears stable enough for everyday use.

  If you experience any problems PLEASE contact me via github.com/milomouse


* Added systemd service script.

  If using systemd; recommend running under user-session@..

    % systemd --user start mifo

    % systemd --user stop mifo

  If not using systemd or if undesired; simply run with..

    % mifo --init

    % mifo --quit
