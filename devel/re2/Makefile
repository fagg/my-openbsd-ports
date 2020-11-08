# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= alternative formatting library for C and C++

GH_ACCOUNT= 	google
GH_PROJECT= 	re2
GH_TAGNAME= 	2020-11-01
CATEGORIES= 	devel
HOMEPAGE=   	

MAINTAINER= 	Ashton Fagg <ashton@fagg.id.au>

# BSD
PERMIT_PACKAGE= Yes

COMPILER= 	base-clang
MODULES=  	devel/cmake

WANTLIB=  	${COMPILER_LIBCXX}

CONFIGURE_ARGS+=-DCMAKE_INSTALL_PREFIX="${PREFIX}" \
		-DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
