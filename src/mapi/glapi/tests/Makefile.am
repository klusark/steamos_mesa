if !HAVE_SHARED_GLAPI
AM_CFLAGS = $(PTHREAD_CFLAGS)
AM_CPPFLAGS = \
	$(DEFINES) \
	-I$(top_srcdir)/src/gtest/include \
	-I$(top_builddir)/src/mapi \
	-I$(top_srcdir)/src/mapi \
	-I$(top_srcdir)/include

TESTS = glapi-test
check_PROGRAMS = glapi-test

glapi_test_SOURCES =			\
	check_table.cpp

glapi_test_LDADD = \
	$(top_builddir)/src/mapi/glapi/libglapi.la \
	$(top_builddir)/src/gtest/libgtest.la \
	$(PTHREAD_LIBS)
endif
