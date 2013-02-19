# Box is full of boxes

> I just *know* I have a Debian box somewhere…

Do you have more than π boxes? Are you constantly forgetting about them?

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

## Who Box is for

Box is designed for managing at most 20 boxes. If you have a large deployment
to manage, we recommend that you check out larger tools like [Ansible][],
 [Salt Stack][], [Chef][] or [Puppet][] (in roughly increasing order of complexity).

## Requirements

Box requires a POSIX sh(1) implementation on boxes and on the machine Box is
run from. Box connects to servers with SSH and assumes that SSH keys are set
up.

## Getting started

    git clone git@github.com:wolverian/box.git
    cd box
    echo user1@host1.com >> etc/hosts
    echo user2@host2.com >> etc/hosts
    PATH=bin:$PATH
    box tasks
    …
    box id
    …

[GNU Parallel]: http://www.gnu.org/software/parallel/
[Salt Stack]: http://saltstack.org
[Chef]: http://www.opscode.com/chef/
[Puppet]: https://puppetlabs.com
[Ansible]: http://ansible.cc
