PORTNAME=	pius-carp
PORTVERSION=	0.4.4
PORTREVISION=	1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	CARP for PIUS

BUILD_DEPENDS=	${LOCALBASE}/include/boost/detail/endian.hpp:${PORTSDIR}/devel/boost-libs
BUILD_DEPENDS+=	pius-netmap>=2.0:${PORTSDIR}/net/pius-netmap
DEPENDS+=	pius-netmap>=2.0:${PORTSDIR}/net/pius-netmap

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
