mifo (2.8)
---------

About:

* MPlayer daemon with preset/native commands controlled through a FIFO.

* Written in ZSH.

* GPL-3 License.

---------

Requirements:

* ZSH

* MPLAYER2 or MPLAYER [not MPV]

* PROCPS (ps|pgrep|pkill)

* COREUTILS (mkfifo)

---------

Query:

* Currently unaware of native Zsh handling for external process collection.

* Currently unaware of native Zsh handling for fifo creation.

* Will *not* support 'mpv' due to altered and handicapped slave command / sub-options.

---------

Notes:

* Script is in its developmental stages although appears stable enough for everyday use.

  If you experience any problems PLEASE contact me via github.com/milomouse


*  Start daemon:

  `mifo --init`

*  Quit daemon:

  `mifo --quit`

* Show help:

  `mifo --help`

* Show detailed help for an option:

  `mifo --OPTION --`

