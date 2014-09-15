PORTNAME=	trafficgen
PORTVERSION=	1.2.2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	mshao@petabi.com
COMMENT=	Traffic generator

LIB_DEPENDS=	liblua-5.2.so:${PORTSDIR}/lang/lua52
LIB_DEPENDS+=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
