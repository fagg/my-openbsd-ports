# $OpenBSD: Makefile.template,v 1.88 2020/05/15 01:32:48 abieber Exp $

COMMENT= 	alternative formatting library for C and C++

GH_ACCOUNT= 	fmtlib
GH_PROJECT= 	fmt
GH_TAGNAME= 	7.1.1

SHARED_LIBS=	flatbuffers	0.0	#1.12

CATEGORIES= 	devel
HOMEPAGE=   	https://github.com/fmtlib/fmt

MAINTAINER= 	Ashton Fagg <ashton@fagg.id.au>

# MIT
PERMIT_PACKAGE= Yes

# C++11
COMPILER= 	 base-clang
MODULES=  	 devel/cmake
WANTLIB=  ${COMPILER_LIBCXX} c pthread

CONFIGURE_ARGS+= -DFMT_PEDANTIC=on \
		 -DFMT_DOC=on \
		 -DFMT_INSTALL=on \
		 -DBUILD_SHARED_LIBS=on

.include <bsd.port.mk>
