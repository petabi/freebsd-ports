PORTNAME=	pius-session
PORTVERSION=	0.21.1
PORTREVISION=	1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Network session management module for PIUS

BUILD_DEPENDS+=	pius-netmap>=2.0.0:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-carp>=0.4.4:${PORTSDIR}/net/pius-carp
BUILD_DEPENDS+=	petabi-ip_tools>=0.2:${PORTSDIR}/net/petabi-ip_tools
LIB_DEPENDS+=	libboost_program_options.so:devel/boost-libs
LIB_DEPENDS+=	libboost_system.so:devel/boost-libs
LIB_DEPENDS+=	liblpm.so:net/petabi-ip_tools

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
