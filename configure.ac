AC_INIT([bric], [m4_esyscmd_s([cat ./.version])], [https://github.com/shnupta/bric/issues], ,[https://github.com/shnupta/bric])
AM_INIT_AUTOMAKE([subdir-objects foreign])
AC_PREREQ(2.69)
AC_CONFIG_HEADERS([src/config.h:config.in])
AC_PROG_CC([cc])
AC_CONFIG_MACRO_DIRS([m4])
AC_PROG_INSTALL

# This prevents problems such as those shown in
# https://github.com/theimpossibleastronaut/rmw/commit/90200c2df06b16f16b5d21d25c51966c0ee65b23#commitcomment-30291627
# and https://github.com/theimpossibleastronaut/rmw/issues/21
AM_MAINTAINER_MODE

AM_GNU_GETTEXT([external], [need-formatstring-macros])
AM_GNU_GETTEXT_VERSION([0.19.8])

# The Makefile.* filenames in po/ are different than the others, and that's intentional,
# according the GNU Gettext documentation.
AC_CONFIG_FILES([       Makefile
			po/Makefile.in])
AC_OUTPUT
