# $FreeBSD$

PORTNAME=	MessagePack
PORTVERSION=	0.3.5
PORTREVISION=	1
CATEGORIES=	devel
PKGNAMEPREFIX=	${LUA_PKGNAMEPREFIX}

MAINTAINER=	oleksii.tsai@gmail.com
COMMENT=	Efficient binary serialization format

BROKEN=		unfetchable
DEPRECATED=	Broken for more than 6 months
EXPIRATION_DATE=	2020-05-05

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/COPYRIGHT

USES=		lua:module
NO_BUILD=	yes
NO_ARCH=	yes

USE_GITHUB=	yes
GH_ACCOUNT=	fperrad
GH_PROJECT=	lua-MessagePack

PLIST_FILES=	%%LUA_MODSHAREDIR%%/${PORTNAME}.lua

do-install:
	${MKDIR} ${STAGEDIR}${LUA_MODSHAREDIR}
	${INSTALL_DATA} ${WRKSRC}/src/${PORTNAME}.lua ${STAGEDIR}${LUA_MODSHAREDIR}

.include <bsd.port.mk>
