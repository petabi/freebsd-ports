# Created by: Jason Harris <jharris@widomaker.com>
# $FreeBSD$

PORTNAME=	units
PORTVERSION=	2.11
CATEGORIES=	math
MASTER_SITES=	GNU

MAINTAINER=	jharris@widomaker.com
COMMENT=	Unit conversion and calculation

LICENSE=	GPLv3

GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--program-prefix=g

INFO=		units

post-patch:
	@${REINPLACE_CMD} -e \
	 's|$$(INSTALL_PROGRAM) units_cur|${INSTALL_SCRIPT} units_cur|' \
	${WRKSRC}/Makefile.in

.include <bsd.port.mk>
