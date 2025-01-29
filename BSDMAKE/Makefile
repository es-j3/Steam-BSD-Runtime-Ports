PORTNAME=       Steam-BSD-Runtime-Ports
PORTVERSION=    1.0.1
CATEGORIES=     games
MASTER_SITES=   https://github.com/es-j3/Steam-BSD-Runtime-Ports/archive/refs/tags/
DISTFILES=      ${PORTVERSION}.tar.gz

MAINTAINER=     alexander.nogal@proton.me
COMMENT=        Steam on FreeBSD, with the help of Proton.


LICENSE=        BSD2CLAUSE
LICENSE_FILE=   ${WRKSRC}/LICENSE

USES=           gmake
NO_ARCH=        yes

# Build and runtime dependencies
BUILD_DEPENDS= 
RUN_DEPENDS=    
# Installation path
PLIST_FILES=    bin/steam-bsd-runtime-uninstaller bin/steam-bsd-runtime-installer

do-build:
	@${ECHO} "Building Steam-BSD-Runtime!"

do-install:
	${INSTALL_SCRIPT} ${WRKSRC}/steam-bsd-runtime-installer ${STAGEDIR}${PREFIX}/bin/steam-bsd-runtime-installer
	${INSTALL_SCRIPT} ${WRKSRC}/steam-bsd-runtime-uninstaller ${STAGEDIR}${PREFIX}/bin/steam-bsd-runtime-uninstaller

.include <bsd.port.mk>
