PORTNAME=	trafficgen
PORTVERSION=	1.2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	mshao@petabi.com
COMMENT=	Traffic generator

LIB_DEPENDS=	liblua-5.2.so:${PORTSDIR}/lang/lua52

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
