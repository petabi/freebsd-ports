PORTNAME=	regorus-sdk
PORTVERSION=	0.2.2
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	kwanghyunk@petabi.com
COMMENT=	Software development kit for REgorus

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
BUILD_DEPENDS+=	rematch>=1.3:${PORTSDIR}/devel/rematch
BUILD_DEPENDS+=	pius-netmap>=1.3:${PORTSDIR}/net/pius-netmap
RUN_DEPENDS+=	rematch>=1.3:${PORTSDIR}/devel/rematch
RUN_DEPENDS+=	pius-netmap>=1.3:${PORTSDIR}/net/pius-netmap

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
