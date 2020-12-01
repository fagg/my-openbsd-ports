# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT=		fast, safe, thread-friendly regular expression engine
CATEGORIES=		textproc
GH_ACCOUNT=		google
GH_PROJECT=		re2
GH_TAGNAME=		2020-11-01
PKGNAME=		re2-${GH_TAGNAME:S,-,,g}

SHARED_LIBS=		re2	0.0

MAINTAINER=		Ashton Fagg <ashton@fagg.id.au>

# BSD
PERMIT_PACKAGE=		Yes

WANTLIB= 		${COMPILER_LIBCXX} m pthread

COMPILER= 		base-clang ports-gcc
MODULES=  		devel/cmake

# Note: One of the regression tests is quite lengthy, and is subject
# to a timelimit enforced by CMake. The default (1500 secs) works on
# the maintainer's machine, but may timeout on slower systems.
CONFIGURE_ARGS+=	-DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
