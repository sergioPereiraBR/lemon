AM_CFLAGS  = -I@top_builddir@/include
AM_LDFLAGS = -L@top_builddir@/src 
LDADD = @LIBS@ -llemon -lm

#
# The programs to build
#
bin_PROGRAMS = lemon_contents lemon_benchmark
check_PROGRAMS = canonical parallel xlf parallel_non_blocking xlf_non_blocking

#
# The program and its dependencies
#
lemon_contents_SOURCES = lemon_contents.c
lemon_benchmark_SOURCES = lemon_benchmark.c md5.c humanForm.c
canonical_SOURCES = canonical.c
parallel_SOURCES = parallel.c
xlf_SOURCES = xlf.c

.PHONY: build_lib
build_lib:
	cd @top_builddir@/lib ; $(MAKE)
