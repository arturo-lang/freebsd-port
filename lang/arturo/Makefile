PORTNAME=       arturo
DISTVERSION=    0.10.0
CATEGORIES=     lang
MASTER_SITES=   https://arturo-lang.io/files/
DISTNAME=       ${PORTNAME}-${DISTVERSION}-freebsd-amd64
EXTRACT_SUFX=   .zip

MAINTAINER=     dr.kameleon@gmail.com
COMMENT=        Simple, expressive & portable programming language
WWW=            https://arturo-lang.io/

LICENSE=        MIT
LICENSE_FILE=   ${WRKSRC}/LICENSE

# Runtime dependencies for full mode
RUN_DEPENDS=    webkit2-gtk3>=0:www/webkit2-gtk3 \
                gtk3>=0:x11-toolkits/gtk3 \
                mpfr>=0:math/mpfr

ONLY_FOR_ARCHS= amd64
NO_BUILD=       yes

PLIST_FILES=    bin/arturo

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/arturo ${STAGEDIR}${PREFIX}/bin/

.include <bsd.port.mk>
