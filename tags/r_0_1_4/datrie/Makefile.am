pkgincludedir = $(includedir)/datrie

pkginclude_HEADERS =	\
	typedefs.h	\
	triedefs.h	\
	trie.h		\
	sb-trie.h

EXTRA_DIST = libdatrie.map

INCLUDES = -I$(top_srcdir)

lib_LTLIBRARIES = libdatrie.la

libdatrie_la_SOURCES =	\
	typedefs.h	\
	triedefs.h	\
	trie-private.h	\
	fileutils.h	\
	fileutils.c	\
	darray.h	\
	darray.c	\
	tail.h		\
	tail.c		\
	trie.h		\
	trie.c		\
	alpha-map.h	\
	alpha-map.c	\
	sb-trie.h	\
	sb-trie.c
libdatrie_la_LDFLAGS =	-no-undefined \
	-version-info $(LT_CURRENT):$(LT_REVISION):$(LT_AGE) \
	-Wl,--version-script=$(srcdir)/libdatrie.map
libdatrie_la_DEPENDENCIES = libdatrie.map

