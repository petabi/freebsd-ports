PORTNAME=	pius
PORTVERSION=	0.5
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Packet Inspection in User Space

BUILD_DEPENDS=	${LOCALBASE}/include/mregex_types.h:${PORTSDIR}/devel/mregex
LIB_DEPENDS=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs

USE_BZIP2=	yes
USES=		cmake

.include <bsd.port.mk>
