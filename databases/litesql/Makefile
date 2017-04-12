# $FreeBSD$

PORTNAME=	litesql
DISTVERSION=	0.3.17rc3
CATEGORIES=	databases devel
MASTER_SITES=	SF/litesql/litesql/${DISTVERSION:S/rc3//}
DISTNAME=	${PORTNAME}-src-${DISTVERSION}

MAINTAINER=	minskim@NetBSD.org
COMMENT=	C++ object persistence framework

LICENSE=	BSD3CLAUSE

LIB_DEPENDS=	libexpat.so:textproc/expat2

USES=		cmake pkgconfig sqlite:3 zip
CMAKE_ARGS+=	-DLITESQL_WITH_TESTS=OFF
#GNU_CONFIGURE=	yes
WRKSRC=		${WRKDIR}/${DISTNAME:S/rc3//}

#CONFIGURE_ARGS+=	--with-expat=${LOCALBASE}
MAKE_JOBS_UNSAFE=yes
#DOCS_BUILD_DEPENDS=	dot:graphics/graphviz
#DOCSDIR=	${PREFIX}/share/doc/${PORTNAME}-${PORTVERSION}

#post-extract:
#	${CHMOD} a+x ${WRKSRC}/configure

#post-patch:
#	@${REINPLACE_CMD} -e 's|-ltermcap|-lncurses|' ${WRKSRC}/configure

.include <bsd.port.mk>
