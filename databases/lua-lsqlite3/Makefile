# $FreeBSD$

PORTNAME=	lsqlite3
PORTVERSION=	0.9.3
DISTFILES=	lsqlite3_fsl09w.zip
CATEGORIES=	databases
PKGNAMEPREFIX=	${LUA_PKGNAMEPREFIX}
MASTER_SITES=	http://lua.sqlite.org/index.cgi/zip/

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Binding for Lua to the SQLite3 database library

LICENSE=	MIT

LIB_DEPENDS=	libsqlite3.so:${PORTSDIR}/databases/sqlite3

WRKSRC=		${WRKDIR}/lsqlite3_fsl09w
USES=		lua

PLIST_FILES=	%%LUA_MODLIBDIR%%/lsqlite3.so

do-build:
	cd ${WRKSRC} &&							\
	${CC} -I${LOCALBASE}/include -I${LOCALBASE}/include/lua52 ${CFLAGS} -fPIC -fms-extensions -c lsqlite3.c && \
	${CC} -shared ${LDFLAGS} -o lsqlite3.so lsqlite3.o -L${LOCALBASE}/lib -llua-5.2 -lsqlite3

do-install:
	@${MKDIR} ${STAGEDIR}${LUA_MODLIBDIR}
	${INSTALL_LIB} ${WRKSRC}/lsqlite3.so ${STAGEDIR}${LUA_MODLIBDIR}/

.include <bsd.port.mk>
