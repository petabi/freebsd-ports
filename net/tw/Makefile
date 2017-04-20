PORTNAME=	tw
PORTVERSION=	0.2.1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	traffic weaver

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
BUILD_DEPENDS+=	auto-opt>=0.2.4:${PORTSDIR}/devel/auto-opt
BUILD_DEPENDS+= rematch>=1.4.5:${PORTSDIR}/devel/rematch
BUILD_DEPENDS+= regorus-sdk>=0.2.1:${PORTSDIR}/net/regorus-sdk
LIB_DEPENDS=	libboost_system.so.1.63.0:${PORTSDIR}/devel/boost-libs
LIB_DEPENDS+=	liblua-5.2.so:${PORTSDIR}/lang/lua52
LIB_DEPENDS+=	libpcre2-8.so:${PORTSDIR}/devel/pcre2

MAKE_JOBS_UNSAFE=	yes

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
