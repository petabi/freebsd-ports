# $FreeBSD$

CATEGORIES=	lang
PKGNAMESUFFIX=	-rtl-console

MAINTAINER=	freebsd-fpc@FreeBSD.org
COMMENT=	Free Pascal console abstraction unit (RTL)

USE_FPC=	rtl-extra

MASTERDIR=	${.CURDIR}/../../lang/fpc
WRKUNITDIR=	${FPCSRCDIR}/packages/${PKGNAMESUFFIX:S/-//}
EXTRACTUNITDIR=	${WRKUNITDIR}

.include "${MASTERDIR}/Makefile"
