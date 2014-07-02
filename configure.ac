#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.68])

AC_INIT([femtolisp],
        [1.0.0],
        [jeff.bezanson@gmail.com],
        [femtolisp],
        [https://github.com/JeffBezanson])

AC_LANG_PUSH([C])
AM_INIT_AUTOMAKE([subdir-objects])
LT_PREREQ([2.4])
LT_INIT([dlopen])
AC_CONFIG_SRCDIR([flmain.c])
AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])

# Checks for programs.
AC_PROG_CC
AC_PROG_MAKE_SET

# Checks for libraries.
AC_CHECK_LIB([m], [cos])

# Checks for header files.
AC_FUNC_ALLOCA
AC_CHECK_HEADERS([fcntl.h limits.h locale.h malloc.h netdb.h netinet/in.h stddef.h stdint.h stdlib.h string.h sys/param.h sys/socket.h sys/time.h sys/timeb.h unistd.h wchar.h wctype.h setjmp.h],[],[AC_MSG_ERROR([missing headers])])

# Checks for typedefs, structures, and compiler characteristics.
AC_C_INLINE

AC_C_BIGENDIAN([AC_DEFINE([BIG_ENDIAN],[1],[define to 1 if big endian])],
               [AC_DEFINE([LITTLE_ENDIAN],[1],[define to 1 if little endian])])

AC_TYPE_INT16_T
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_INT8_T
AC_TYPE_OFF_T
AC_TYPE_PID_T
AC_TYPE_SIZE_T
AC_TYPE_SSIZE_T
AC_CHECK_SIZEOF([void *])

# this is autoconf v2.69
dnl AC_CHECK_HEADER_STDBOOL 

# this is autoconf v2.68
AC_HEADER_STDBOOL

AC_TYPE_UINT16_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_TYPE_UINT8_T

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_MKTIME
AC_FUNC_REALLOC
AC_FUNC_STRTOD

AC_CHECK_FUNCS([bzero floor ftime getcwd gethostbyname gettimeofday iswprint localtime_r memchr memmove memset pow select setenv setlocale socket sqrt strcasecmp strchr strdup strpbrk strrchr strtol strtoull wcwidth])

AC_CONFIG_FILES([Makefile])

AC_OUTPUT
