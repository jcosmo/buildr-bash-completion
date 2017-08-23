buildr-bash-completion
======================

bash completion script for buildr

bash-completion: http://bash-completion.alioth.debian.org/
buildr: http://buildr.apache.org/

Knows the options via _parse_help, and can figure out buildr tasks.

Caches a copy of the possible build tasks based on the current directory.
This has the undesirable sideeffect of not noticing a change in the possible build tasks if you change the buildfile.  Right now the only workaround is to open a new shell (or run buildr in a different directory)

Install:
    cp buildr_bash_expansion.sh /etc/bash_completion.d/buildr
    (may need to source /etc/bash_completion.d/buildr)

Or if you use a local .bash.d directory:
    cp buildr_bash_expansion.sh ~/.bash.d

TODO:
* Expire the cache periodically?
* Look for the possible buildfile in more than the current directory

