# $OpenBSD: Makefile,v 1.46 2021/12/09 16:21:25 jturner Exp $

COMMENT =	functional and imperative programming language
CATEGORIES =	lang

GH_ACCOUNT =	janet-lang
GH_PROJECT =	janet
GH_TAGNAME =	v1.19.2

SHARED_LIBS +=	janet		7.0 # 1.19

HOMEPAGE =	https://www.janet-lang.org/
MAINTAINER =	James Turner <james@calminferno.net>

# MIT
PERMIT_PACKAGE =	Yes

WANTLIB += c m pthread

# Needs TLS
COMPILER =	base-clang ports-gcc
COMPILER_LANGS =	c

USE_GMAKE =	Yes
MAKE_FLAGS =	PREFIX="${PREFIX}" CFLAGS="${CFLAGS}" \
		JANET_LIBRARY="build/libjanet.so.${LIBjanet_VERSION}"

.include <bsd.port.mk>
