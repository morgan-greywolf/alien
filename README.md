# Alien
Please read alien's man page for general documentation.

## Getting alien:

  The original version of alien is still available at the alien home page; drop by
  http://kitenet.net/~joey/code/alien/
  
  But I have no idea for how much longer.

## Other things you'll need:

  To use alien, you will need several other programs. Alien is a perl
  program, and requires perl version 5.004 or greater. If you use slackware,
  make sure you get perl 5.004, the perl 5.003 in slackware does not work
  with alien!

  To convert packages to or from rpms, you need the Red Hat Package Manager;
  get it from Red Hat's ftp site. If your distribution (eg, Red Hat)
  provides a rpm-build package, you will need it as well to generate rpms.

  If you want to convert packages into debian packages, you will need the
  dpkg, dpkg-dev, and debhelper (version 3 or above) packages, which are
  available on http://packages.debian.org

  To convert to/from stampede packages, you will need bzip2.

  Attention, Slackware, Red Hat, and Stampede users: Bruce S. Babcock
  <babcock@math.psu.edu> has put together an "alien-extra"
  package of all the extra files you need to use alien on
  a Red Hat or Slackware system. (Debian systems automatically have all
  required files.)
  
  The Slackware version is at 
  	ftp://ykbsb2.yk.psu.edu/pub/alien/alien-extra.tgz
  The RedHat version is at
  	ftp://ykbsb2.yk.psu.edu/pub/alien/alien-extra.rpm
  The Stampede version is at
  	ftp://ykbsb2.yk.psu.edu/pub/alien/alien-extra.slp

## Note:

  Alien is really designed to be used to convert from alien file formats to
  the packaging format used by the distribution you run it on. Of course,
  it can also convert from your distribution's native format to alien
  formats, or from one alien format to another. Do be warned though, that
  if these latter types of conversions are done, the generated packages may
  have incorrect dependancy information. This is known to be true if you
  convert a rpm into a deb on a Red Hat system, for example. Even with
  alien-extra installed, dpkg will be unable to properly calculate library
  dependancies for the deb it is creating, and you will get a package
  without any library dependancies.

## Programs that use alien:

  I know of one program that acts as a frontend to alien - kpackviewer is a
  package viewer that can convert between package formats by using alien. Its
  homepage is at http://www.momentus.com.br/users/hook/kpackviewer.html

  Corel also appears to have (or had) something in Corel linux that
  uses alien.

## Please report any bugs in alien here. 

  It is helpful to provide a log of alien --veryverbose reproducing the
  bug. I may also ask for the package that exposes the problem you saw.
