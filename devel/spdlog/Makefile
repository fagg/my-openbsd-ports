# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= Fast logging library for C++

GH_ACCOUNT= gabime
GH_PROJECT= spdlog
GH_TAGNAME= v1.8.1
CATEGORIES= devel
HOMEPAGE= https://github.com/gabime/spdlog

MAINTAINER= Ashton Fagg <ashton@fagg.id.au>

# MIT
PERMIT_PACKAGE= Yes

# C++11
COMPILER= base-clang
MODULES= devel/cmake
WANTLIB= ${COMPILER_LIBCXX}

CONFIGURE_ARGS+=-DCMAKE_INSTALL_PREFIX="${PREFIX}" \
	-DSPDLOG_BUILD_TESTS=on \
	-DSPDLOG_BUILD_SHARED=on

.include <bsd.port.mk>
