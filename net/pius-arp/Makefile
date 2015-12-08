PORTNAME=	pius-arp
PORTVERSION=	1.3
PORTREVISION=	2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	ARP and NDP for PIUS

BUILD_DEPENDS=	${LOCALBASE}/include/boost/detail/endian.hpp:${PORTSDIR}/devel/boost-libs

USES=		cmake tar:bzip2

CMAKE_ARGS+=	-DBUILD_SHARED_LIBS=ON

.include <bsd.port.mk>
