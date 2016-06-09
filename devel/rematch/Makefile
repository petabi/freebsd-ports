PORTNAME=	rematch
PORTVERSION=	1.4.2
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Regular expression matching library

BUILD_DEPENDS+=	llvm38>=3.8.0:${PORTSDIR}/devel/llvm38
BUILD_DEPENDS+=	pius-carp>=0.1.1:${PORTSDIR}/net/pius-carp
BUILD_DEPENDS+=	pius-netmap>=1.0:${PORTSDIR}/net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.17.3:${PORTSDIR}/net/pius-session
LIB_DEPENDS+=	libpcre2-8.so:${PORTSDIR}/devel/pcre2

MAKE_JOBS_UNSAFE=	yes

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
