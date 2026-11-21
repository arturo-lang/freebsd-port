PORTNAME=	arturo
DISTVERSION=	0.10.0
CATEGORIES=	lang
MASTER_SITES=	https://arturo-lang.io/files/
DISTNAME=	${PORTNAME}-${DISTVERSION}-freebsd-amd64

MAINTAINER=	dr.kameleon@gmail.com
COMMENT=	Simple, expressive & portable programming language
WWW=		https://arturo-lang.io/

LICENSE=	MIT

ONLY_FOR_ARCHS=	amd64

# Runtime dependencies for full mode
RUN_DEPENDS=	webkit2-gtk>=0:www/webkit2-gtk \
		gtk30>=0:x11-toolkits/gtk30 \
		mpfr>=0:math/mpfr

USES=		zip

NO_BUILD=	yes

PLIST_FILES=	bin/arturo

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/arturo ${STAGEDIR}${PREFIX}/bin/

.include <bsd.port.mk>
