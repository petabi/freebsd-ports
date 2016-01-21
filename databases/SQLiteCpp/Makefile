# $FreeBSD$

PORTNAME=	SQLiteCpp
PORTVERSION=	1.2.0
PORTREVISION=	1
CATEGORIES=	databases

MAINTAINER=	ports@FreeBSD.org
COMMENT=	C++ SQLite3 wrapper

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

USE_GITHUB=	yes
GH_ACCOUNT=	SRombauts

USES=		cmake
USE_SQLITE=	3
CMAKE_ARGS+=	-DCMAKE_CXX_FLAGS:STRING="-I${LOCALBASE}/include"

PLIST_FILES=	include/SQLiteCpp/Assertion.h \
		include/SQLiteCpp/Column.h \
		include/SQLiteCpp/Database.h \
		include/SQLiteCpp/Exception.h \
		include/SQLiteCpp/SQLiteCpp.h \
		include/SQLiteCpp/Statement.h \
		include/SQLiteCpp/Transaction.h \
		lib/libSQLiteCpp.a

do-install:
	${MKDIR} ${STAGEDIR}${PREFIX}/include/SQLiteCpp
	${INSTALL_DATA} ${WRKSRC}/include/SQLiteCpp/* ${STAGEDIR}${PREFIX}/include/SQLiteCpp/
	${INSTALL_DATA} ${WRKSRC}/libSQLiteCpp.a ${STAGEDIR}${PREFIX}/lib/

.include <bsd.port.mk>
