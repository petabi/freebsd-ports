PORTNAME=	pius
PORTVERSION=	0.13
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Packet Inspection in User Space

BUILD_DEPENDS+=	mregex>=1.0.4:${PORTSDIR}/devel/mregex
BUILD_DEPENDS+= pius-arp>=1.2:${PORTSDIR}/net/pius-arp
BUILD_DEPENDS+=	pius-netmap>=0.2:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.14.2:${PORTSDIR}/net/pius-session
LIB_DEPENDS=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	liblua-5.2.so:${PORTSDIR}/lang/lua52

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
