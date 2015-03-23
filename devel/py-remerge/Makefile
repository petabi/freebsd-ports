PORTNAME=	remerge
PORTVERSION=	0.9.6
CATEGORIES=	devel python
MASTER_SITES=	# empty
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	msk@petabi.com
COMMENT=	Utility to merge similar regular expressions

LIB_DEPENDS=	libpcre.so:${PORTSDIR}/devel/pcre

USE_PYTHON=		3
USE_PYDISTUTILS=	yes
PYDISTUTILS_AUTOPLIST= 	yes

CPPFLAGS+=	$$(${PCRE_CONFIG} --cflags)
LDFLAGS+=	$$(${PCRE_CONFIG} --libs)

PCRE_CONFIG?=	${LOCALBASE}/bin/pcre-config

.include <bsd.port.mk>
