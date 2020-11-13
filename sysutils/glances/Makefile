# $OpenBSD$

COMMENT =		cross-platform curses-based monitoring tool

MODPY_EGG_VERSION =	3.1.5

DISTNAME =		Glances-${MODPY_EGG_VERSION}
PKGNAME =		${DISTNAME:L}

CATEGORIES =		sysutils

HOMEPAGE =		https://nicolargo.github.io/glances

MAINTAINER =		Ashton Fagg <ashton@fagg.id.au>

# LGPLv3
PERMIT_PACKAGE =	Yes

MODULES =		lang/python
MODPY_VERSION=		${MODPY_DEFAULT_VERSION_3}

MODPY_PI =		Yes
MODPY_SETUPTOOLS =	Yes
RUN_DEPENDS=		sysutils/py-psutil${MODPY_FLAVOR} \
			devel/py-future${MODPY_FLAVOR}


.include <bsd.port.mk>
