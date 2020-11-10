# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT=		alternative formatting library for C and C++

GH_ACCOUNT=		google
GH_PROJECT=		re2
GH_TAGNAME=		2020-11-01
CATEGORIES=		devel

MAINTAINER=		Ashton Fagg <ashton@fagg.id.au>

# BSD
PERMIT_PACKAGE=		Yes

COMPILER= 		base-clang ports-gcc
MODULES=  		devel/cmake

WANTLIB+= 		${COMPILER_LIBCXX} c++ c++abi m pthread

CONFIGURE_ARGS+=	-DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
