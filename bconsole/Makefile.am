##############################################################################
## $Id: Makefile.am,v 1.9 2004/04/13 08:42:08 behdad Exp $
## $Author: behdad $
## $Date: 2004/04/13 08:42:08 $
## $Revision: 1.9 $
## $Source: /home/arabeyes/cvs/projects/bicon/bconsole/Makefile.am,v $
##############################################################################
##                                               -*- Automake -*-
## Process this file with automake to produce Makefile.in

pkglib_LTLIBRARIES = libbconsole.la

libbconsole_la_SOURCES = \
		bconsole_ligature.c \
		bconsole_log2con.c
libbconsole_la_LIBADD = \
		$(top_builddir)/bjoining/libbjoining.la

pkginclude_HEADERS = \
		bconsole_ligature.h \
		bconsole_log2con.h \
		bconsole.h

TABLE_FILES = \
		bconsole_lig.i \
		bconsole_nsm_shape.i

EXTRA_DIST = \
		$(TABLE_FILES)

noinst_PROGRAMS = bconsole_vu

AM_CPPFLAGS = \
		$(FRIBIDI_CFLAGS) \
		-I$(top_srcdir)/bjoining

LDADD = \
		libbconsole.la $(FRIBIDI_LIBS)

-include $(top_srcdir)/git.mk
