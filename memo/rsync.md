# Rsync archive on cygwin

rsync.exe --chmod=ugo=rwX --progress -a --size-only --delete src dest

* -a copy everything from time to metadata
* --chmod=ugo=rwX to translate rights on dest (otherwise no body can open files)
* --size-only because time is not perfect
