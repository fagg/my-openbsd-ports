# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT=		alternative formatting library for C and C++

GH_ACCOUNT=		fmtlib
GH_PROJECT=		fmt
GH_TAGNAME=		7.1.3

SHARED_LIBS=		fmt	0.0

CATEGORIES=		devel

MAINTAINER=		Ashton Fagg <ashton@fagg.id.au>

# MIT
PERMIT_PACKAGE=		Yes

# C++11
COMPILER=		base-clang ports-gcc
MODULES=		devel/cmake
WANTLIB+=		c++ c++abi ${COMPILER_LIBCXX}


CONFIGURE_ARGS+=	-DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
