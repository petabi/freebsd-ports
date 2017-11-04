PORTNAME=	pius
PORTVERSION=	0.15
PORTREVISION=	2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Packet Inspection in User Space

BUILD_DEPENDS+=	auto-opt>=0.2.3:${PORTSDIR}/devel/auto-opt
BUILD_DEPENDS+= pius-arp>=1.2:${PORTSDIR}/net/pius-arp
BUILD_DEPENDS+=	pius-netmap>=2.0:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.14.2:${PORTSDIR}/net/pius-session
BUILD_DEPENDS+=	rematch>=1.3:${PORTSDIR}/devel/rematch
BUILD_DEPENDS+=	regorus-sdk>=0.2:${PORTSDIR}/net/regorus-sdk
BUILD_DEPENDS+=	thrift>=0.9.3:${PORTSDIR}/devel/thrift
LIB_DEPENDS=	libboost_system.so:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	liblua-5.2.so:${PORTSDIR}/lang/lua52
LIB_DEPENDS+=   libpius-carp.so:${PORTSDIR}/net/pius-carp
LIB_DEPENDS+=   libthrift-0.9.3.so:${PORTSDIR}/devel/thrift-cpp

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
