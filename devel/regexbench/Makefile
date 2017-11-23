PORTNAME=	regexbench
PORTVERSION=	0.2.2
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	connor@petabi.com
COMMENT=	Regular expression benchmark tool

BUILD_DEPENDS=  rematch>=1.3:devel/rematch
LIB_DEPENDS=    libboost_system.so:devel/boost-libs
LIB_DEPENDS+=   libre2.so:devel/re2
LIB_DEPENDS+=   libhs.so:devel/hyperscan

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
