# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= 	memory optimized serialization library

GH_ACCOUNT= 	google
GH_PROJECT= 	flatbuffers
GH_TAGNAME= 	v1.12.0
CATEGORIES= 	devel
HOMEPAGE=   	https://google.github.io/flatbuffers/

MAINTAINER= 	Ashton Fagg <ashton@fagg.id.au>

# Apache 2
PERMIT_PACKAGE= Yes

# Both base and ports lang seems to have problems compiling code-gen'd
# code produced for the test suite. It's not clear why, and has
# possibly already been fixed upstream.  Ash to investigate.
COMPILER= 	ports-gcc
MODULES=  	devel/cmake
WANTLIB=  	${COMPILER_LIBCXX}

SHARED_LIBS+= 	flatbuffers-1.12.0  1.12.0

CONFIGURE_ARGS+=-DCMAKE_INSTALL_PREFIX="${PREFIX}" \
		-DFLATBUFFERS_BUILD_SHAREDLIB=on \
		-DFLATBUFFERS_BUILD_TESTS=on \
		-DFLATBUFFERS_BUILD_FLATLIB=off

.include <bsd.port.mk>
