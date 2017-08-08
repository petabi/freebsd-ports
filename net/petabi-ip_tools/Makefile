PORTNAME=	petabi-ip_tools
PORTVERSION=	0.2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	connor@petabi.com
COMMENT=	Petabi development IP Tools

LIB_DEPENDS+=	libboost_system.so.1.63.0:${PORTSDIR}/devel/boost-libs

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
