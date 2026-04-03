SUBDIRS = common include libfiry src

check_SCRIPTS = temp/greptest.sh
TESTS = $(check_SCRIPTS)

temp/greptest.sh:
	echo './src/memfiry | grep "Hello from .*memfiry!"' > temp/greptest.sh
	chmod +x temp/greptest.sh

CLEANFILES = temp/greptest.sh

ACLOCAL_AMFLAGS = -I m4
