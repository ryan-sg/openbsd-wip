# $OpenBSD: Makefile,v 1.9 2017/10/27 07:21:11 ajacoutot Exp $

COMMENT =	KDE file search and metadata handling framework
VERSION =	15.04.26
DISTNAME =	baloo-${VERSION}
PKGNAME =	kf5-${DISTNAME}
REVISION =	5

SHARED_LIBS =	KF5Baloo		1.0
SHARED_LIBS +=	KF5BalooXapian		1.0

#
# Modern version requires LMDB, see databases/openldap/Makefile,
# so we create our own tarball with sources for repository revision
# cc72568cb2262355fd53745ea61ba8554bc87466
#
# Warning: if other frameworks will start to depend on baloo,
# kf5.port.mk auto-kf5-dep-versioning will need adjusting.
#

MASTER_SITES =	http://www.ohvost.ru/dnl/
EXTRACT_SUFX =	.tar.gz

WANTLIB += ${COMPILER_LIBCXX} KF5Auth KF5Bookmarks KF5Codecs KF5Completion
WANTLIB += KF5ConfigCore KF5ConfigGui KF5ConfigWidgets KF5CoreAddons
WANTLIB += KF5Crash KF5DBusAddons KF5FileMetaData KF5GuiAddons
WANTLIB += KF5I18n KF5IconThemes KF5IdleTime KF5ItemViews KF5JobWidgets
WANTLIB += KF5KDELibs4Support KF5KIOCore KF5KIOFileWidgets KF5KIOWidgets
WANTLIB += KF5Notifications KF5Parts KF5Service KF5Solid KF5SonnetUi
WANTLIB += KF5TextWidgets KF5UnitConversion KF5WidgetsAddons KF5WindowSystem
WANTLIB += KF5XmlGui Qt5Core Qt5DBus Qt5Gui Qt5Network Qt5PrintSupport
WANTLIB += Qt5Qml Qt5Sql Qt5Widgets Qt5Xml c m xapian

BUILD_DEPENDS =	devel/gettext-tools

RUN_DEPENDS =	x11/dbus,-suid \
		x11/gtk+3,-guic

LIB_DEPENDS =	databases/xapian-core \
		devel/kf5/kauth \
		devel/kf5/kconfig \
		devel/kf5/kcrash \
		devel/kf5/kdbusaddons \
		devel/kf5/kdelibs4support<=5.39.0 \
		devel/kf5/kfilemetadata \
		devel/kf5/ki18n \
		devel/kf5/kidletime \
		devel/kf5/kio \
		devel/kf5/solid \
		x11/qt5/qtdeclarative

CONFIGURE_ARGS +=	-DCMAKE_POLICY_DEFAULT_CMP0063=OLD

# TODO: The following tests FAILED:
#         11 - filewatchtest (Failed)
#         18 - schedulertest (Failed)
#         19 - extractortest (Failed)
#
# TODO: implement filewatch.cpp using QFileSystemWatcher

PORTHOME =		${WRKDIR}
TEST_IS_INTERACTIVE =	X11

.include <bsd.port.mk>
