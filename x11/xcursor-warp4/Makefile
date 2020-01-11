# $OpenBSD$

PKG_ARCH =		*

COMMENT =		black xcursor theme

V =			0.1.0
DISTNAME =		${GH_PROJECT}-${V}
PKGNAME =		xcursor-warp4-${V}

GH_ACCOUNT =		ps1-ch
GH_PROJECT =		warp4xcursors
GH_TAGNAME =		v${V}

CATEGORIES =		x11

# License
PERMIT_PACKAGE =	Yes
PERMIT_DISTFILES =	Yes

BUILD_DEPENDS=  x11/xcursorgen>=7

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/lib/X11/icons/warp4/cursors
	${INSTALL_DATA} ${WRKSRC}/cursors/* ${PREFIX}/lib/X11/icons/warp4/cursors

.include <bsd.port.mk>
