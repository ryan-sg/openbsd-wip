# $OpenBSD: Makefile,v 1.6 2017/10/26 08:24:17 rsadowski Exp $

SUBDIR =
SUBDIR += extra-cmake-modules	# 100% tests passed, 0 tests failed out of 50

# do not sort blindly: items below are listed in the straight build order

# tier 1
SUBDIR += ki18n			# 100% tests passed, 0 tests failed out of 5
SUBDIR += attica		# 100% tests passed, 0 tests failed out of 1
SUBDIR += bluez-qt 		# NO_TEST
SUBDIR += breeze-icons		# 75% tests passed, 1 tests failed out of 4
SUBDIR += kapidox		# NO_TEST
SUBDIR += karchive		# 80% tests passed, 1 tests failed out of 5
SUBDIR += kcodecs		# 100% tests passed, 0 tests failed out of 6
SUBDIR += kconfig		# 100% tests passed, 0 tests failed out of 35
SUBDIR += kcoreaddons		# 96% tests passed, 1 tests failed out of 23
SUBDIR += kdbusaddons		# stucks
SUBDIR += kdnssd		# NO_TEST
SUBDIR += kguiaddons		# 100% tests passed, 0 tests failed out of 3
SUBDIR += kidletime		# NO_TEST
SUBDIR += kitemmodels		# 100% tests passed, 0 tests failed out of 11
SUBDIR += kitemviews		# 100% tests passed, 0 tests failed out of 1
SUBDIR += kplotting		# 100% tests passed, 0 tests failed out of 4
SUBDIR += kwidgetsaddons	# 100% tests passed, 0 tests failed out of 18
SUBDIR += kwindowsystem		# 62% tests passed, 5 tests failed out of 13
SUBDIR += oxygen-icons		# 67% tests passed, 1 tests failed out of 3
SUBDIR += solid			# 75% tests passed, 1 tests failed out of 4
SUBDIR += sonnet		# 100% tests passed, 0 tests failed out of 4
SUBDIR += threadweaver		# 100% tests passed, 0 tests failed out of 7
SUBDIR += syntax-highlighting	# 100% tests passed, 0 tests failed out of 8
SUBDIR += prison		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kirigami2		# 

# tier 2
SUBDIR += kauth			# 100% tests passed, 0 tests failed out of 2
SUBDIR += kcompletion		# 100% tests passed, 0 tests failed out of 4
SUBDIR += kcrash		# 50% tests passed, 1 tests failed out of 2
SUBDIR += kdoctools		# 100% tests passed, 0 tests failed out of 1S
SUBDIR += kfilemetadata		# 92% tests passed, 1 tests failed out of 13
SUBDIR += kimageformats		# 8% tests passed, 12 tests failed out of 13
SUBDIR += kjobwidgets		# NO_TEST
SUBDIR += knotifications	# 100% tests passed, 0 tests failed out of 1
SUBDIR += kpty			# stucks
SUBDIR += kunitconversion	# 100% tests passed, 0 tests failed out of 3
SUBDIR += kpackage		# 90% tests passed, 1 tests failed out of 10

# tier 3
# high contention on [kservice..kio..kdeclarative] path, be careful
SUBDIR += kservice		# 40% tests passed, 6 tests failed out of 10
SUBDIR += kconfigwidgets	# 100% tests passed, 0 tests failed out of 3
SUBDIR += kiconthemes		# 100% tests passed, 0 tests failed out of 7
SUBDIR += kpeople		# 100% tests passed, 0 tests failed out of 3
SUBDIR += kwallet		# 100% tests passed, 0 tests failed out of 1
SUBDIR += kemoticons		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kglobalaccel		# 100% tests passed, 0 tests failed out of 1
SUBDIR += ktextwidgets		# 100% tests passed, 0 tests failed out of 5
SUBDIR += kxmlgui		# 80% tests passed, 1 tests failed out of 5
SUBDIR += kbookmarks		# 100% tests passed, 0 tests failed out of 1
SUBDIR += kdesu			# NO_TEST
SUBDIR += kio			# 93% tests passed, 4 tests failed out of 54
SUBDIR += knewstuff		# 100% tests passed, 0 tests failed out of 3
SUBDIR += kactivities		# NO_TEST
SUBDIR += kinit			# NO_TEST
SUBDIR += kactivities-stats	# NO_TEST
SUBDIR += kparts		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kded			# NO_TEST
SUBDIR += kxmlrpcclient		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kdeclarative		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kcmutils		# NO_TEST
SUBDIR += kdewebkit		# NO_TEST
SUBDIR += baloo			# 79% tests passed, 4 tests failed out of 19
SUBDIR += kdesignerplugin	# 100% tests passed, 0 tests failed out of 2
SUBDIR += knotifyconfig		# NO_TEST
SUBDIR += ktexteditor		# 98% tests passed, 1 tests failed out of 66
SUBDIR += plasma-framework	# 50% tests passed, 7 tests failed out of 14
SUBDIR += krunner		# 50% tests passed, 1 tests failed out of 2

# tier 4
SUBDIR += frameworkintegration	# 100% tests passed, 0 tests failed out of 1

# porting aids
SUBDIR += kdelibs4support	# stucks
SUBDIR += khtml			# 100% tests passed, 0 tests failed out of 2
SUBDIR += kjs			# 100% tests passed, 0 tests failed out of 1
SUBDIR += kjsembed		# NO_TEST
SUBDIR += kmediaplayer		# 100% tests passed, 0 tests failed out of 2
SUBDIR += kross			# 100% tests passed, 0 tests failed out of 1

# corresponding software isn't ported
#SUBDIR += modemmanager-qt
#SUBDIR += network-manager-qt
#SUBDIR += kwayland

.include <bsd.port.subdir.mk>
