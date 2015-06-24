PORTNAME=	regorus-sdk
PORTVERSION=	0.2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	kwanghyunk@petabi.com
COMMENT=	Software development kit for REgorus

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
DEPENDS+=	rematch>=1.3:${PORTSDIR}/devel/rematch
DEPENDS+=	pius-netmap>=1.3:${PORTSDIR}/net/pius-netmap

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
