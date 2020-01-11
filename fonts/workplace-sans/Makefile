# $OpenBSD$

COMMENT =		semi-condensed sans-serif font

V =			102
DISTNAME =		wpsu_bit_$V
PKGNAME =		workplace-sans-$V

CATEGORIES =		fonts

HOMEPAGE =		http://www.altsan.org/creative/fonts/workplace/

# SIL OFL 1.1
PERMIT_PACKAGE =	Yes
PERMIT_DISTFILES =	Yes

MASTER_SITES =		http://www.altsan.org/creative/fonts/workplace/ http://hobbes.nmsu.edu/download/pub/multimedia/fonts/truetype/
EXTRACT_SUFX =		.zip

NO_BUILD =		Yes

FONTDIR =		${PREFIX}/share/fonts/workplace-sans
FCDIR =			${PREFIX}/share/workplace-sans

do-install:
	${INSTALL_DATA_DIR} ${FONTDIR} ${FCDIR}
	${INSTALL_DATA} ${WRKDIR}/*.{ttf,flg,txt} ${FONTDIR}
	${INSTALL_DATA} ${FILESDIR}/30-workplace-sans-aliases.conf ${FCDIR}

.include <bsd.port.mk>
