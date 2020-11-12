# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT=		fast, safe, thread-friendly regular expression engine
CATEGORIES=		devel
GH_ACCOUNT=		google
GH_PROJECT=		re2
GH_TAGNAME=		2020-11-01
DISTNAME=		re2-${GH_TAGNAME}

# This is needed because otherwise the package build pukes due to it
# not understanding the versioning convention.
PKGNAME=		re2-${GH_TAGNAME:S,-,,g}

SHARED_LIBS=		libre2	0.0

MAINTAINER=		Ashton Fagg <ashton@fagg.id.au>

# BSD
PERMIT_PACKAGE=		Yes

COMPILER= 		base-clang ports-gcc
MODULES=  		devel/cmake

WANTLIB= 		${COMPILER_LIBCXX} m pthread

CONFIGURE_ARGS+=	-DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
