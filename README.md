### Bashmarks is a shell script that allows you to save and jump to commonly used directories. Now supports tab completion.

### Modifications
This is a fork of <https://github.com/huyng/bashmarks.git>, with the command names switched out for a set that I'd gotten used to when I'd grown a similar concept out of a bash function/alias.

## Install

1. git clone git://github.com/yumaikas/bashmarks.git
2. cd bashmarks
3. make install
4. source **~/.local/bin/bashmarks.sh** from within your **~.bash\_profile** or **~/.bashrc** file

## Shell Commands

    jadd <bookmark_name> - Saves the current directory as "bookmark_name"
    j <bookmark_name> - Goes (cd) to the directory associated with "bookmark_name"
    jp <bookmark_name> - Prints the directory associated with "bookmark_name"
    jrm <bookmark_name> - Deletes the bookmark
    jl                 - Lists all available bookmarks
    
## Example Usage

    $ cd /var/www/
    $ jadd webfolder
    $ cd /usr/local/lib/
    $ jadd locallib
    $ jl
    $ j web<tab>
    $ j webfolder

## Where Bashmarks are stored
    
All of your directory bookmarks are saved in a file called ".sdirs" in your HOME directory.
