# $OpenBSD: Makefile,v 1.5 2017/10/26 07:53:23 rsadowski Exp $

COMMENT =		KDE icon GUI utility library
DISTNAME =		kiconthemes-${VERSION}

SHARED_LIBS =		KF5IconThemes		3.0

WANTLIB += ${COMPILER_LIBCXX} KF5Archive KF5Auth KF5Codecs KF5ConfigCore
WANTLIB += KF5ConfigGui KF5ConfigWidgets KF5CoreAddons KF5I18n
WANTLIB += KF5ItemViews KF5WidgetsAddons Qt5Core Qt5DBus Qt5Gui
WANTLIB += Qt5Svg Qt5Widgets Qt5Xml c m

MODULES =		lang/python

BUILD_DEPENDS =		devel/gettext-tools

LIB_DEPENDS =		devel/kf5/karchive \
			devel/kf5/kconfigwidgets \
			devel/kf5/kcoreaddons \
			devel/kf5/ki18n \
			devel/kf5/kitemviews \
			devel/kf5/kwidgetsaddons \
			x11/qt5/qtsvg

TEST_IS_INTERACTIVE =	X11
PORTHOME =		${WRKDIR}

.include <bsd.port.mk>
