AC_INIT([ipmid], [0.1], [openbmc@lists.ozlabs.org])

AM_INIT_AUTOMAKE([-Wall -Werror foreign])

AM_SILENT_RULES([yes])

AC_PROG_CXX
AX_CXX_COMPILE_STDCXX_11

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_FILES([Makefile])

AC_SEARCH_LIBS([dlopen], [dl], [], [
		AC_MSG_ERROR(["unable to find dlopen()"])
])

AC_SEARCH_LIBS([sd_bus_message_read], [systemd], [], [
		AC_MSG_ERROR(["unable to find systemd"])
])

AC_OUTPUT
