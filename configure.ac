AC_INIT(picomodel, 0.8.20, picomodel@github)
AC_CONFIG_AUX_DIR(config)
AC_CONFIG_SRCDIR(src/picomodel.c)

AM_INIT_AUTOMAKE
AC_SUBST(VERSION)

AC_PROG_CC
AC_PROG_LIBTOOL
AC_PROG_INSTALL
AC_HEADER_STDC

# libm
AC_CHECK_LIB(m, sqrt,, [AC_MSG_ERROR([requires math library])])
MATH_LIBS=-lm
AC_SUBST(MATH_LIBS)

LT_INIT

AC_OUTPUT(
	Makefile
	src/Makefile
	libpicomodel.pc
)