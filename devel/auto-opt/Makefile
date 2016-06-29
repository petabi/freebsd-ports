PORTNAME=	auto-opt
PORTVERSION=	0.2
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Configuration library using Lua

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
BUILD_DEPENDS+=	${LOCALBASE}/include/boost/fusion/container/map.hpp:${PORTSDIR}/devel/boost-libs
BUILD_DEPENDS+=	${LOCALBASE}/include/lua52/lua.h:${PORTSDIR}/lang/lua52
RUN_DEPENDS+=	${LOCALBASE}/include/boost/fusion/container/map.hpp:${PORTSDIR}/devel/boost-libs
RUN_DEPENDS+=	${LOCALBASE}/include/lua52/lua.h:${PORTSDIR}/lang/lua52

USES=		cmake tar:bzip2

.include <bsd.port.mk>
