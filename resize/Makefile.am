#
#	Makefile.am (30.03.15)
#	Automake source.
#
#	Free exFAT implementation.
#	Copyright (C) 2011-2018  Andrew Nayenko
#
#	This program is free software; you can redistribute it and/or modify
#	it under the terms of the GNU General Public License as published by
#	the Free Software Foundation, either version 2 of the License, or
#	(at your option) any later version.
#
#	This program is distributed in the hope that it will be useful,
#	but WITHOUT ANY WARRANTY; without even the implied warranty of
#	MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#	GNU General Public License for more details.
#
#	You should have received a copy of the GNU General Public License along
#	with this program; if not, write to the Free Software Foundation, Inc.,
#	51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
#

sbin_PROGRAMS = resize_exfat
dist_man8_MANS = resize_exfat.8
mkexfatfs_SOURCES = \
	cbm.c \
	cbm.h \
	fat.c \
	fat.h \
	main.c \
	resize_exfat.c \
	resize_exfat.h \
	rootdir.c \
	rootdir.h \
	uct.c \
	uct.h \
	uctc.c \
	uctc.h \
	vbr.c \
	vbr.h
mkexfatfs_CPPFLAGS = -I$(top_srcdir)/libexfat
mkexfatfs_LDADD = ../libexfat/libexfat.a

install-exec-hook:
	ln -sf $(sbin_PROGRAMS) $(DESTDIR)$(sbindir)/resize_exfat

uninstall-hook:
	rm -f $(DESTDIR)$(sbindir)/resize_exfat
