mifo (2.8)
---------

About:

* MPlayer daemon with preset/native commands controlled through a FIFO.

* Written in ZSH.

* BSD-2 License.

---------

Requirements:

* ZSH

* MPLAYER2 or MPLAYER [not MPV]

* PROCPS (ps|pgrep|pkill)

* COREUTILS (mkfifo)

---------

Notes:

* Will *not* support 'mpv' due to altered and handicapped slave command / sub-options.

* Script is in its developmental stages although appears stable enough for everyday use.

  ( If you experience any problems PLEASE contact me via github.com/milomouse )

* Currently unaware of native Zsh handling for external process collection.

* Currently unaware of native Zsh handling for fifo creation.

---------

Operation:

*  Initiate daemon:

  `mifo --init`

*  Quit daemon:

  `mifo --quit`

* Show help:

  `mifo --help`

  `mifo --`

* Show detailed help for an option:

  `mifo --OPTION --`

---------

Full Command List:

`mifo 2.8 [2014-02-06] (C) 2010-2014 Vincent ZaGara II`

```
  usage: mifo [option] [[arg(s)]]

  common options:
    -l,  --load       Load file(s)/dir(s) and restart playback
    -L,  --append     Append file(s)/dir(s) and keep playback
    -b,  --begin      Begin playback; [*list][file][last]
    -t,  --toggle     Toggle playback; [pause,unpause]
    -n,  --next       Play next file; [(integer),keyword]
    -p,  --prev       Play prev file; [(integer),keyword]
    -r,  --repeat     Repeat current file; [on,off,(integer)]
    -s,  --seek       Seek to position; (integer) [0,1,2]
    -x,  --random     Play a random file in current playlist
    -a,  --announce   Announce current file information
    -w,  --watch      Watch current playing and print changes
    -o,  --show       Show contents of playlist
    -O,  --shown      Show contents of playlist with count(s)
    -f,  --find       Find matches in current playlist
    -F,  --findn      Find matches in current.. with count(s)
    -m,  --mute       Toggle audio muting; [mute,unmute]
    -c,  --command    Send MPlayer command to the daemon
    -h,  --help       Display this message and exit

  extended options:
    -pa, --add        Add current file to a playlist
    -pr, --remove     Remove current file from a playlist
    -pc, --check      Check if current file is in a playlist
    -ps, --save       Save current playlist as a new playlist
    -pe, --edit       Edit a saved playlist
    -pl, --playlist   Load a saved playlist
    -pp, --printp     Display saved playlists

  long options only:
         --instance   Check if daemon is active/running or not
         --stop       Stop playback but keep daemon active
         --quit       Close daemon, unless already closed
         --init       Start daemon, unless already started
         --version    Display current MPlayer and mifo versions

  You may also type "OPTION --" for help specific to OPTION.
```

