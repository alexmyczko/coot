
lib_LTLIBRARIES=libcoot-AngleInfo.la

EXTRA_DIST = \
	angle-torsion-autogen.awk

pkginclude_HEADERS = AngleInfo.h ncube.h wrapped-ncube.h
pkgincludedir = $(includedir)/coot/angles

AM_CPPFLAGS = $(CLIPPER_CXXFLAGS)

libcoot_AngleInfo_a_sources = AngleInfo.cc AngleInfo.h  \
	AngleInfo-angle-torsions-autogen.cc AngleInfo-theta_2-autogen.cc

libcoot_AngleInfo_la_SOURCES = $(libcoot_AngleInfo_a_sources)

# needed to get past (some) g++ compilers.  Details forgotten.
libcoot_AngleInfo_la_CXXFLAGS = -g -O1

libcoot_AngleInfo_la_LDFLAGS = $(SHARED_LDFLAGS)

# bin_PROGRAMS = test_angle
# test_angle_SOURCES = test-angle.cc
# test_angle_LDADD = -L. -lmapview-AngleInfo

