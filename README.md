# Perl versions on the Mac

Apple lists the open source they use, so I trawled through that to
extract the versions of Perl that each Mac version shipped with.

Some notes:

* I can't verify most of this because I don't have these old systems
* Apple may have modified the perl
* Apple distributes some extra stuff, too
* In some versions, Apple ships multiple perls
* Try `man perlmacosx` for Apple-specific details

There's also
[tsibley/apple-perl-versions](https://github.com/tsibley/apple-perl-versions),
but that doesn't include the point release information for
each perl, and in may cases seems to disagree with what Apple declares
and people have reported. It also stops at OS X 10.13.

The list from
[Barry Walsh](https://transfixedbutnotdead.com/2010/02/03/perl-and-mac-os-x-versions/)
is a bit better, but dated. A lot of this is verified in
[comments on StackOverflow](https://stackoverflow.com/questions/2092944/how-can-i-find-out-which-perl-version-was-available-on-older-mac-os-x-versions).

There's even [a list on cpan.org](https://www.cpan.org/ports/binaries.html#mac_osx),
but it doesn't include the internal build numbers or the second (or
third) version that shipped. Well, not yet but [I sent a pull request](https://github.com/perlorg/cpanorg/pull/52).

If you have corrections or more information, raise an issue or send a
pull request.
