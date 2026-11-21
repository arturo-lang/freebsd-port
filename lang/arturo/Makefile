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

LIB_DEPENDS=	libgmp.so:math/gmp \
		libiconv.so:converters/libiconv \
		libmpfr.so:math/mpfr \
		libsoup-3.0.so:devel/libsoup3 \
		libwebkit2gtk-4.1.so:www/webkit2-gtk@41

USES=		gnome xorg zip
USE_GNOME=	atk cairo gdkpixbuf glib20 gtk30 pango
USE_XORG=	xcb

NO_BUILD=	yes
NO_WRKSUBDIR=	yes

PLIST_FILES=	bin/arturo

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/arturo ${STAGEDIR}${PREFIX}/bin/

.include <bsd.port.mk>
