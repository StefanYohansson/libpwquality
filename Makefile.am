#
# Copyright (c) 2005, 2006, 2007 Thorsten Kukuk <kukuk@thkukuk.de>
# Copyright (c) 2011 Red Hat, Inc.
# Copyright (c) 2011 Tomas Mraz <tm@t8m.info>
#

AUTOMAKE_OPTIONS = 1.9 gnu dist-bzip2 check-news

SUBDIRS = po src doc
if BUILD_PYTHON_BINDINGS
SUBDIRS += python
endif

CLEANFILES = *~

M4_FILES = m4/libtool.m4

EXTRA_DIST = config.rpath $(M4_FILES) libpwquality.spec libpwquality.spec.in

ACLOCAL_AMFLAGS = -I m4

tag: Makefile
	hg tag libpwquality-@PACKAGE_VERSION@

force-tag: Makefile
	hg tag -f libpwquality-@PACKAGE_VERSION@
