noinst_LIBRARIES = common/libjupcommon.a
common_libjupcommon_a_SOURCES = common/libjupcommon.h common/print.c

bin_PROGRAMS = bin/memfiry
bin_memfiry_SOURCES = src/main.c
bin_memfiry_CPPFLAGS = -I$(top_srcdir)/common
bin_memfiry_LDADD = common/libjupcommon.a

check_SCRIPTS = temp/greptest.sh
TESTS = $(check_SCRIPTS)

temp/greptest.sh:
	echo './bin/memfiry | grep "Hello from .*memfiry!"' > temp/greptest.sh
	chmod +x temp/greptest.sh

CLEANFILES = temp/greptest.sh
