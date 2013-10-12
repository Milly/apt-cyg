apt-cyg
=======

Fork of [apt-cyg](http://code.google.com/p/apt-cyg/) from http://code.google.com/p/apt-cyg/

Intro
-----
apt-cyg is a command-line installer for Cygwin which cooperates with Cygwin Setup and uses the same repository. The syntax is similar to apt-get. Usage examples:

* "apt-cyg install <package names>" to install packages
* "apt-cyg reinstall <package names>" to reinstall packages
* "apt-cyg remove <package names>" to remove packages
* "apt-cyg mirrors" to show mirrors
* "apt-cyg update" to update setup.ini
* "apt-cyg show" to show installed packages
* "apt-cyg find <pattern(s)>" to find packages matching patterns
* "apt-cyg search <pattern(s)>" (alias of find)
* "apt-cyg describe <pattern(s)>" to describe packages matching patterns
* "apt-cyg info <pattern(s)>" (alias of describe)
* "apt-cyg packageof <commands or files>" to locate parent packages

Quick start
-----------
First install curl and wget through the standard cygwin setup program. Then run the following commands:

    # curl -o /usr/bin/apt-cyg https://raw.github.com/milly/apt-cyg/master/apt-cyg
    # chmod +x /usr/bin/apt-cyg

use apt-cyg, for example:

    # apt-cyg update
    # apt-cyg install nano

Command completion
------------------
apt-cyg has command completion in zsh.

    # curl -o /usr/share/zsh/site-functions/_apt-cyg https://raw.github.com/milly/apt-cyg/master/zsh_completion/_apt-cyg
    # autoload -Uz compinit && compinit -u
