PORTNAME=	mregex
PORTVERSION=	1.1.1
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Regular expression matching library

BUILD_DEPENDS+=	pius-carp>=0.1.1:${PORTSDIR}/net/pius-carp
BUILD_DEPENDS+=	pius-netmap>=0.2:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.14.2:${PORTSDIR}/net/pius-session

MAKE_JOBS_UNSAFE=	yes

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
