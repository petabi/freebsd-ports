PORTNAME=	rematch
PORTVERSION=	1.3
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Regular expression matching library

BUILD_DEPENDS+=	pius-carp>=0.1.1:${PORTSDIR}/net/pius-carp
BUILD_DEPENDS+=	pius-netmap>=1.0:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.17.3:${PORTSDIR}/net/pius-session

MAKE_JOBS_UNSAFE=	yes

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
