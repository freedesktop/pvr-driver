# Copyright (c) 2011 Intel Corporation. All Rights Reserved.
#
# Permission is hereby granted, free of charge, to any person obtaining a
# copy of this software and associated documentation files (the
# "Software"), to deal in the Software without restriction, including
# without limitation the rights to use, copy, modify, merge, publish,
# distribute, sub license, and/or sell copies of the Software, and to
# permit persons to whom the Software is furnished to do so, subject to
# the following conditions:
# 
# The above copyright notice and this permission notice (including the
# next paragraph) shall be included in all copies or substantial portions
# of the Software.
# 
# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
# OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT.
# IN NO EVENT SHALL PRECISION INSIGHT AND/OR ITS SUPPLIERS BE LIABLE FOR
# ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
#
AC_PREREQ(2.57)
AC_INIT([psb-video], 0.1, [waldo.bastian@intel.com], psb-video)
AC_CONFIG_SRCDIR([Makefile.am])
AM_INIT_AUTOMAKE([dist-bzip2])

AM_CONFIG_HEADER([src/config.h])

AC_DISABLE_STATIC
AC_PROG_LIBTOOL
AC_PROG_CC

AC_HEADER_STDC
AC_SYS_LARGEFILE

PKG_CHECK_MODULES([X11], [x11])
PKG_CHECK_MODULES([XEXT], [xext])
PKG_CHECK_MODULES([DRM], [libdrm])
PKG_CHECK_MODULES([WSBM], [libwsbm])
PKG_CHECK_MODULES([LIBVA], [libva])
PKG_CHECK_MODULES([XV], [xv])

pkgconfigdir=${libdir}/pkgconfig
AC_SUBST(pkgconfigdir)

AC_OUTPUT([Makefile src/Makefile fw/Makefile])
