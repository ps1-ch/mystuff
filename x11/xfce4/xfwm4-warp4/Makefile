# $OpenBSD$

PKG_ARCH =		*

COMMENT =		window decoration theme for xfwm4

V =			0.1.0
DISTNAME =		${GH_PROJECT}-${V}
PKGNAME =		xfwm4-warp4-${V}

GH_ACCOUNT =		ps1-ch
GH_PROJECT =		warp4xfwm4
GH_TAGNAME =		v${V}

CATEGORIES =		x11

# License
PERMIT_PACKAGE =	Yes
PERMIT_DISTFILES =	Yes

NO_BUILD =		Yes

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/themes/warp4/xfwm4
	${INSTALL_DATA} ${WRKDIR}/${DISTNAME}/warp4/xfwm4/* ${PREFIX}/share/themes/warp4/xfwm4

.include <bsd.port.mk>
