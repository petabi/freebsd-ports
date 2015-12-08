PORTNAME=	pius
PORTVERSION=	0.14.1
PORTREVISION=	1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Packet Inspection in User Space

BUILD_DEPENDS+= pius-arp>=1.2:${PORTSDIR}/net/pius-arp
BUILD_DEPENDS+=	pius-netmap>=1.3:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.14.2:${PORTSDIR}/net/pius-session
BUILD_DEPENDS+=	rematch>=1.3:${PORTSDIR}/devel/rematch
BUILD_DEPENDS+=	regorus-sdk>=0.2:${PORTSDIR}/net/regorus-sdk
LIB_DEPENDS=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	liblua-5.2.so:${PORTSDIR}/lang/lua52

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
