PORTNAME=	trafficgen
PORTVERSION=	1.2.2
PORTREVISION=	2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	mshao@petabi.com
COMMENT=	Traffic generator

LIB_DEPENDS=	liblua-5.2.so:${PORTSDIR}/lang/lua52
LIB_DEPENDS+=	libboost_system.so.1.60.0:${PORTSDIR}/devel/boost-libs

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
