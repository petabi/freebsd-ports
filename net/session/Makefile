PORTNAME=	session
PORTVERSION=	0.12.1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Network session management module for PIUS

LIB_DEPENDS+=	libboost_system.so.1.55.0:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	libboost_program_options.so.1.55.0:${PORTSDIR}/devel/boost-libs

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
