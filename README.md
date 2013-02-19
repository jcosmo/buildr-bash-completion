buildr-bash-completion
======================

bash completion script for buildr

bash-completion: http://bash-completion.alioth.debian.org/
buildr: http://buildr.apache.org/

Knows the options via _parse_help, and can figure out
buildr tasks.

Install:
    cp buildr /etc/bash_completion.d/

    (may need to source /etc/bash_completion.d/buildr)



Kind of klugey at the moment, our buildfile includes
ant tasks for checkstyle, which ends up loading a
handful of pom.xml and generally being a touch
slow, so there is a klugey hack to skip that
and specify 'checkstyle' directly.
