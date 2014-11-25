PORTNAME=	pius
PORTVERSION=	0.11
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Packet Inspection in User Space

BUILD_DEPENDS=	${LOCALBASE}/include/mregex_types.h:${PORTSDIR}/devel/mregex
BUILD_DEPENDS+= libpius-arp.a:${PORTSDIR}/net/pius-arp
LIB_DEPENDS=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	liblua-5.2.so:${PORTSDIR}/lang/lua52

USE_BZIP2=	yes
USES=		cmake

.include <bsd.port.mk>
