PORTNAME=	pius-netmap
PORTVERSION=	1.6.1
CATEGORIES=	net
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Utilities to access netmap buffer

BUILD_DEPENDS+=	atf>=0.21:${PORTSDIR}/devel/atf
BUILD_DEPENDS+=	${LOCALBASE}/include/boost/lockfree/spsc_queue.hpp:${PORTSDIR}/devel/boost-libs
RUN_DEPENDS+=	${LOCALBASE}/include/boost/lockfree/spsc_queue.hpp:${PORTSDIR}/devel/boost-libs

USES=		cmake tar:bzip2

.include <bsd.port.mk>
