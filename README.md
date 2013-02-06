# Box is full of boxes

Do you have more than π boxes? Are you constantly forgetting about them? Does
this sound familiar: “I just *know* I have a Debian box somewhere…”? If you answered
yes, perhaps Box is for you!

With Box you can easily:

- Keep inventory of your boxes!

        $ box ls
        foo.bar.com
        bar.baz.net
        quux.org

- Ping them!

        $ box ping
        foo.bar.com: available
        bar.baz.net: unreachable
        quux.org: available

- Remind yourself what you put in those boxes!

        $ box id
        foo.bar.com: Arch Linux
        bar.baz.net: Ubuntu 12.04 LTS
        quux.org: NetBSD 6.0.1

All this and more, for the low price of *nothing*! Get Box today!

## Overview

Box is a remote command execution program. Box allows you to run commands on
all of your remote servers and presents the produced results in a readable
format.

In the future, Box will likely morph into a (still minimal) configuration
management system.

## Dependencies

Box requires a POSIX sh(1) implementation on boxes and on the machine Box is
run from. Box connects to servers with SSH and assumes that SSH keys are set
up.

At the moment, Box requires [GNU Parallel][]. This dependency might be
relaxed.

[GNU Parallel]: http://www.gnu.org/software/parallel/
