# Created by: clsung
# $FreeBSD$

PORTNAME=	Net-Domain-ExpireDate
PORTVERSION=	1.15.2
CATEGORIES=	dns net perl5
MASTER_SITES=	CPAN
MASTER_SITE_SUBDIR=	CPAN:NALOBIN
PKGNAMEPREFIX=	p5-

MAINTAINER=	perl@FreeBSD.org
COMMENT=	Perl module obtain expiration date of domain names

BUILD_DEPENDS=	p5-Net-Whois-Raw>=0:net/p5-Net-Whois-Raw
RUN_DEPENDS:=	${BUILD_DEPENDS}

NO_ARCH=	yes
USES=		perl5
USE_PERL5=	configure
WRKSRC=		${WRKDIR}/${PORTNAME}-${PORTVERSION:R}

.include <bsd.port.mk>
