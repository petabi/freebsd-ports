PORTNAME=	rematch
PORTVERSION=	1.7
CATEGORIES=	devel
MASTER_SITES=	# empty

MAINTAINER=	msk@petabi.com
COMMENT=	Regular expression matching library

BUILD_DEPENDS+=	llvm38>=3.8.0:devel/llvm38
BUILD_DEPENDS+=	pius-carp>=0.1.1:net/pius-carp
BUILD_DEPENDS+=	pius-netmap>=2.0:net/pius-netmap
BUILD_DEPENDS+=	pius-session>=0.18.0:net/pius-session
LIB_DEPENDS+=	libboost_filesystem.so:devel/boost-libs
LIB_DEPENDS+=	libboost_program_options.so:devel/boost-libs
LIB_DEPENDS+=	libboost_system.so:devel/boost-libs
LIB_DEPENDS+=	libpcre2-8.so:devel/pcre2
LIB_DEPENDS+=	libpius-carp.so:net/pius-carp
LIB_DEPENDS+=	libpius-session.so:net/pius-session

MAKE_JOBS_UNSAFE=	yes

USES=		cmake tar:bzip2

CFLAGS+=	-DNDEBUG

.include <bsd.port.mk>
