[![Build Status](https://travis-ci.com/skaji/perl6-build.svg?branch=master)](https://travis-ci.com/skaji/perl6-build)

# NAME

Perl6::Build - build rakudo Perl6

# SYNOPSIS

    Usage:
     $ perl6-build [options] VERSION   PREFIX [-- [configure options]]
     $ perl6-build [options] COMMITISH PREFIX [-- [configure options]]

    Options:
     -h, --help      show this help
     -l, --list      list available versions (latest 20 versions)
     -L, --list-all  list all available versions
     -w, --workdir   set working directory, default: ~/.perl6-build
         --jvm       build perl6 with jvm backend

    Example:
     # List available versions
     $ perl6-build -l

     # Build and install rakudo-star-2018.04 to ~/perl6
     $ perl6-build rakudo-star-2018.04 ~/perl6

     # Build and install rakudo from git repository (2018.06 tag) to ~/perl6
     $ perl6-build 2018.06 ~/perl6

     # Build and install rakudo from git repository (HEAD) to ~/perl6-{describe}
     # where {describe} will be replaced by `git describe` such as `2018.06-259-g72c8cf68c`
     $ perl6-build HEAD ~/perl6-'{describe}'

     # Build and install rakudo from git repository (HEAD) with jvm backend
     $ perl6-build --jvm 2018.06 ~/2018.06-jvm

     # Build and install rakudo from git repository (2018.06 tag) with custom configure options
     $ perl6-build 2018.06 ~/2018.06-custom -- --backends moar --with-nqp /path/to/bin/nqp

# INSTALLATION

There are 3 ways:

- CPAN

        $ cpm install -g Perl6::Build

- Self-contained version

        $ wget https://raw.githubusercontent.com/skaji/perl6-build/master/bin/perl6-build
        $ chmod +x perl6-build
        $ ./perl6-build --help

- As a p6env plugin

        $ git clone https://github.com/skaji/perl6-build ~/.p6env/plugins/perl6-build
        $ p6env install -l

    See [https://github.com/skaji/p6env](https://github.com/skaji/p6env).

# DESCRIPTION

Perl6::Build builds rakudo Perl6.

# AUTHOR

Shoichi Kaji <skaji@cpan.org>

# COPYRIGHT AND LICENSE

Copyright 2018 Shoichi Kaji <skaji@cpan.org>

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.
