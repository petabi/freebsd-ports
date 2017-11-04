PORTNAME=	reconvergelite
PORTVERSION=	0.3
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	atsuzuki@petabi.com
COMMENT=	Event Correlation System

BUILD_DEPENDS=  rematch>=1.3:devel/rematch
BUILD_DEPENDS+= thrift>=0.9.3:devel/thrift
LIB_DEPENDS=    libboost_system.so:devel/boost-libs
LIB_DEPENDS+=   liblua-5.2.so:lang/lua52
LIB_DEPENDS+=   libthrift-0.9.3.so:devel/thrift-cpp
LIB_DEPENDS+=   libboost_python.so.1.63.0:devel/boost-python-libs

MAKE_JOBS_UNSAFE=	yes

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
