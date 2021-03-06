[![Build Status](https://travis-ci.com/skaji/perl6-build.svg?branch=master)](https://travis-ci.com/skaji/perl6-build)

# NAME

Perl6::Build - build rakudo Perl6

# SYNOPSIS

    $ perl6-build [options] VERSION   PREFIX [-- [configure options]]
    $ perl6-build [options] COMMITISH PREFIX [-- [configure options]]

See [perl6-build](https://metacpan.org/pod/distribution/Perl6-Build/script/perl6-build).

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
