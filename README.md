# Perl versions on the Mac

Apple lists the open source they use, so I trawled through that to
extract the versions of Perl that each Mac version shipped with.

* [Apple perl distros on GitHub](https://github.com/apple-oss-distributions/perl)
* [Open source projects in macOS releases](https://opensource.apple.com/releases/)

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

## Switching perls

Since Catalina, macOS ships with more than one version of perl. There's
a default version noted in the JSON.

Change the perl version through the `VERSIONER_PERL_VERSION` environment
variable using the major and minor version:

	% export VERSIONER_PERL_VERSION=5.34

I give a [longer example on Stackoverflow](https://stackoverflow.com/a/75968566/2766176).

## Source

The primary repository is in GitHub, but as with most of my stuff, I
mirror the repo in several services in case of outage or other situation
where one might not exist:

* [GitHub](https://github.com/briandfoy/mac-perl-versions)
* [Bitbucket](https://bitbucket.org/briandfoy/mac-perl-versions/)
* [Gitlab](https://gitlab.com/briandfoy/mac-perl-versions)
* [Codeberg](https://codeberg.org/briandfoy/mac-perl-versions)

