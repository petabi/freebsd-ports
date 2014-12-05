PORTNAME=	mregex
PORTVERSION=	1.0.2
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Regular expression matching library

BUILD_DEPENDS+=	${LOCALBASE}/include/session_table.h:${PORTSDIR}/net/session

MAKE_JOBS_UNSAFE=	yes

USE_BZIP2=	yes
USES=		cmake

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
