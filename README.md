mifo (2.6)
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


*  Start daemon:

    % mifo --init

*  Quit daemon:

    % mifo --quit

* Show help:

    % mifo --help

* Show detailed help for an option:

    % mifo --OPTION --

