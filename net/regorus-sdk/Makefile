PORTNAME=	regorus-sdk
PORTVERSION=	0.1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	kwanghyunk@petabi.com
COMMENT=	Software development kit for REgorus

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
BUILD_DEPENDS+=	mregex>=1.0.4:${PORTSDIR}/devel/mregex
DEPENDS+=	pius-netmap>=1.3:${PORTSDIR}/net/pius-netmap

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
