PORTNAME=	pius-carp
PORTVERSION=	0.1.1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	CARP for PIUS

BUILD_DEPENDS=	${LOCALBASE}/include/boost/detail/endian.hpp:${PORTSDIR}/devel/boost-libs

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
