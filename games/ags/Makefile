# $OpenBSD$

COMMENT =	adventure game studio engine

V =		3.4.3.1
DISTNAME =	ags-v.${V}
PKGNAME =	ags-${V}
CATEGORIES =	games

HOMEPAGE =	http://www.adventuregamestudio.co.uk/

# Artistic 2.0
PERMIT_PACKAGE =	Yes
PERMIT_DISTFILES =	Yes

WANTLIB =		X11 c freetype m pthread stdc++ alleg ogg theora vorbis vorbisfile

MASTER_SITES =		https://github.com/adventuregamestudio/ags/

DISTFILES =		ags-{archive/}v.${V}${EXTRACT_SUFX}

BUILD_DEPENDS =		audio/dumb
LIB_DEPENDS =		games/allegro audio/libogg multimedia/libtheora audio/libvorbis

USE_GMAKE =		Yes
COMPILER =		ports-gcc
COMPILER_LANGS =	c

WRKSRC =		${WRKDIR}/${DISTNAME}/Engine

pre-build:
	cp ${FILESDIR}/Makefile-defs.obsd ${WRKSRC}

.include <bsd.port.mk>
