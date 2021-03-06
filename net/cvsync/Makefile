# $FreeBSD$

PORTNAME=	cvsync
PORTVERSION=	0.25.0
DISTVERSION=	0.24.19
CATEGORIES=	net ipv6
MASTER_SITES=	ftp://ftp.cvsync.org/pub/cvsync/ \
		ftp://ftp.allbsd.org/pub/cvsync/

MAINTAINER=	hrs@FreeBSD.org
COMMENT=	Portable CVS repository synchronization utility

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/doc/COPYRIGHT

USES=		gmake
USE_RC_SUBR=	cvsyncd
USE_OPENSSL=	yes

PORTDOCS=	ChangeLog FAQ TODO
PORTEXAMPLES=	cvsync.conf cvsyncd-FreeBSD.conf \
		cvsyncd-NetBSD.conf cvsyncd-OpenBSD.conf

MAKE_ENV+=	DESTDIR="${STAGEDIR}" \
		PTHREAD_LIBS="-lpthread" \
		INSTALL= \
		INSTALL_BIN_OPTS="${INSTALL_PROGRAM}" \
		INSTALL_MAN_OPTS="${INSTALL_MAN}"
MAKE_FLAGS=	OSVER="${OSVERSION}" HASH_TYPE=openssl

OPTIONS_DEFINE=	DOCS EXAMPLES

post-install-EXAMPLES-on:
	@${MKDIR} ${STAGEDIR}${EXAMPLESDIR}
	cd ${WRKSRC}/samples && ${INSTALL_DATA} ${PORTEXAMPLES} ${STAGEDIR}${EXAMPLESDIR}

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	cd ${WRKSRC}/doc && ${INSTALL_DATA} ${PORTDOCS} ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
