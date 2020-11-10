# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= alternative formatting library for C and C++

GH_ACCOUNT= 	google
GH_PROJECT= 	bloaty
GH_TAGNAME= 	v1.1
CATEGORIES= 	devel
HOMEPAGE=   	https://github.com/google/bloaty

MAINTAINER= 	Ashton Fagg <ashton@fagg.id.au>

# Apache 2
PERMIT_PACKAGE= Yes

# C++11
COMPILER= 	base-clang ports-gcc
MODULES=  	devel/cmake

WANTLIB=  	${COMPILER_LIBCXX} \
		protobuf \
		capstone \
		re2

LIB_DEPENDS=    devel/protobuf \
		devel/capstone/main \
		devel/re2

CONFIGURE_ARGS+=-DCMAKE_INSTALL_PREFIX="${PREFIX}"

.include <bsd.port.mk>
