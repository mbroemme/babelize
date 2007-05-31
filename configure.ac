# The autoconf initilization.
AC_INIT(babelize, 1.1.0, [mbroemme@plusserver.de], [babelize])

# Detect the canonical host and target build environment
AC_CANONICAL_SYSTEM

AM_INIT_AUTOMAKE([no-dependencies])
AC_CONFIG_HEADERS([config.h:config.h.in])

# Notices
AC_PREREQ(2.53)
AC_REVISION($Revision: 1.6 $)

# Exporting some required variables.
AC_PATH_PROG([bashpath], [bash], [no])
if test "$bashpath" = "no"; then
	AC_MSG_ERROR([bash binary is required])
fi
AC_PATH_PROG([basenamepath], [basename], [no])
if test "$basenamepath" = "no"; then
	AC_MSG_ERROR([basename binary is required])
fi
AC_PATH_PROG([dirnamepath], [dirname], [no])
if test "$dirnamepath" = "no"; then
	AC_MSG_ERROR([dirname binary is required])
fi
AC_PATH_PROG([cppath], [cp], [no])
if test "$cppath" = "no"; then
	AC_MSG_ERROR([cp binary is required])
fi
AC_PATH_PROG([rmpath], [rm], [no])
if test "$rmpath" = "no"; then
	AC_MSG_ERROR([rm binary is required])
fi
AC_PATH_PROG([mvpath], [mv], [no])
if test "$mvpath" = "no"; then
	AC_MSG_ERROR([mv binary is required])
fi
AC_PATH_PROG([chmodpath], [chmod], [no])
if test "$chmodpath" = "no"; then
	AC_MSG_ERROR([chmod binary is required])
fi
AC_PATH_PROG([greppath], [grep], [no])
if test "$greppath" = "no"; then
	AC_MSG_ERROR([grep binary is required])
fi
AC_PATH_PROG([sedpath], [sed], [no])
if test "$sedpath" = "no"; then
	AC_MSG_ERROR([sed binary is required])
fi
AC_PATH_PROG([mkdirpath], [mkdir], [no])
if test "$mkdirpath" = "no"; then
	AC_MSG_ERROR([mkdir binary is required])
fi
AC_PATH_PROG([findpath], [find], [no])
if test "$findpath" = "no"; then
	AC_MSG_ERROR([find binary is required])
fi
AC_PATH_PROG([md5sumpath], [md5sum], [no])
if test "$md5sumpath" = "no"; then
	AC_MSG_ERROR([md5sum binary is required])
fi
AC_PATH_PROG([tarpath], [tar], [no])
if test "$tarpath" = "no"; then
	AC_MSG_ERROR([tar binary is required])
fi
AC_PATH_PROG([xdeltapath], [xdelta], [no])
if test "$xdeltapath" = "no"; then
	AC_MSG_ERROR([xdelta binary is required])
fi
AC_PATH_PROG([statpath], [stat], [no])
if test "$statpath" = "no"; then
	AC_MSG_ERROR([stat binary is required])
fi

# Creating files.
AC_OUTPUT([
Makefile
bin/Makefile
etc/Makefile
share/babelize/Makefile
share/man/Makefile
])
