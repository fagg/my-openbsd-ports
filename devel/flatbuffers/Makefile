# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= memory optimized serialization library

GH_ACCOUNT= google
GH_PROJECT= flatbuffers
GH_TAGNAME= v1.12.0
CATEGORIES= devel
HOMEPAGE=   https://google.github.io/flatbuffers/

MAINTAINER= Ashton Fagg <ashton@fagg.id.au>

# Apache 2
PERMIT_PACKAGE= Yes

COMPILER= ports-gcc
MODULES=  devel/cmake
WANTLIB=  ${COMPILER_LIBCXX}

CONFIGURE_ARGS+=-DCMAKE_INSTALL_PREFIX="${PREFIX}" \
				-DFLATBUFFERS_BUILD_SHAREDLIB=on \
				-DFLATBUFFERS_BUILD_TESTS=on \
				-DFLATBUFFERS_BUILD_FLATLIB=off

.include <bsd.port.mk>
