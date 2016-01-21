# $FreeBSD$

PORTNAME=	lrexlib-pcre
PORTVERSION=	2.7.2
DISTVERSION=	rel-2-7-2
CATEGORIES=	devel
PKGNAMEPREFIX=	${LUA_PKGNAMEPREFIX}

MAINTAINER=	ports@FreeBSD.org
COMMENT=	PCRE regexp library for Lua (lrexlib project)

LICENSE=	MIT

LIB_DEPENDS=	libpcre.so:${PORTSDIR}/devel/pcre

USES=		libtool:build lua

USE_GITHUB=	yes
GH_PROJECT=	lrexlib
GH_ACCOUNT=	rrthomas

CFLAGS+=	-fPIC -DVERSION=\"2.7.2\"

PLIST_FILES=	%%LUA_MODLIBDIR%%/rex_pcre.a %%LUA_MODLIBDIR%%/rex_pcre.so %%LUA_MODLIBDIR%%/rex_pcre.so.0 %%LUA_MODLIBDIR%%/rex_pcre.so.0.0.0

do-build:
	cd ${WRKSRC} && \
	libtool --tag=CC --mode=compile ${CC} -fms-extensions -I${LOCALBASE}/include/lua52 -c ${CFLAGS} src/common.c  && \
	libtool --tag=CC --mode=compile ${CC} -fms-extensions -I${LOCALBASE}/include/lua52 -I${LOCALBASE}/include -c ${CFLAGS} src/pcre/lpcre.c && \
	libtool --tag=CC --mode=compile ${CC} -fms-extensions -I${LOCALBASE}/include/lua52 -I${LOCALBASE}/include -c ${CFLAGS} src/pcre/lpcre_f.c && \
	libtool --tag=CC --mode=link ${CC} -o rex_pcre.la -L${LOCALBASE}/lib -lpcre -llua-5.2 common.lo lpcre.lo lpcre_f.lo \
		-module -version-info 0:0 -rpath ${LOCALBASE}/lib

do-install:
	@${MKDIR} ${STAGEDIR}${LUA_MODLIBDIR}
	libtool --mode=install ${INSTALL_LIB} ${WRKSRC}/rex_pcre.la ${STAGEDIR}${LUA_MODLIBDIR}/

.include <bsd.port.mk>
