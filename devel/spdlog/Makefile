# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= Fast logging library for C++

GH_ACCOUNT= gabime
GH_PROJECT= spdlog
GH_TAGNAME= v1.8.1
CATEGORIES= devel

SHARED_LIBS=	spdlog	0.0

MAINTAINER= Ashton Fagg <ashton@fagg.id.au>

# MIT
PERMIT_PACKAGE= Yes

# C++11
COMPILER= base-clang ports-gcc
MODULES= devel/cmake

LIB_DEPENDS= devel/fmt

WANTLIB+= c++ c++abi m pthread ${COMPILER_LIBCXX}

CONFIGURE_ARGS+= -DSPDLOG_BUILD_TESTS=on \
		-DSPDLOG_BUILD_SHARED=on \
		-DSPDLOG_FMT_EXTERNAL=on

.include <bsd.port.mk>
