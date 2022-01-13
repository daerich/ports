# $OpenBSD: Makefile,v 1.2 2019/07/12 20:49:53 sthen Exp $

COMMENT =	truncate or extend the length of files
V = 5.2.1
PKGNAME = truncate-${V}
CATEGORIES =	sysutils

HOMEPAGE =	https://www.dragonflybsd.org/
MAINTAINER =	Brian Callahan <bcallah@openbsd.org>

# BSD
PERMIT_PACKAGE =	Yes

WANTLIB += c

pre-build:
.for _FILE in Makefile truncate.c truncate.1
	@cp ${FILESDIR}/${_FILE} ${WRKBUILD}
.endfor

.include <bsd.port.mk>
