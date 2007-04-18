# The top-level input Makefile for mpq-tools

# minimum required automake 1.6
AUTOMAKE_OPTIONS = 1.6

# architecture-independent script files
babelizedir = $(bindir)
babelize_DATA = babelize babelize-config

EXTRA_DIST = $(babelize_DATA)
 
install-data-hook:
	$(sedpath) 's,@BABELIZE_VERSION@,$(PACKAGE_VERSION),' -i ${babelizedir}/babelize
	$(sedpath) 's,SYSCONFDIR=.*,SYSCONFDIR="$(sysconfdir)",' -i ${babelizedir}/babelize
	$(sedpath) 's,DATADIR=.*,DATADIR="$(datadir)",' -i ${babelizedir}/babelize
	$(sedpath) 's,@BASH@,${bashpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@BABELIZE_VERSION@,$(PACKAGE_VERSION),' -i ${babelizedir}/babelize-config
	$(sedpath) 's,SYSCONFDIR=.*,SYSCONFDIR="$(sysconfdir)",' -i ${babelizedir}/babelize-config
	$(sedpath) 's,DATADIR=.*,DATADIR="$(datadir)",' -i ${babelizedir}/babelize-config
	$(sedpath) 's,@BASH@,${bashpath},' -i ${babelizedir}/babelize-config
	$(sedpath) 's,@BASENAME@,${basenamepath},' -i ${babelizedir}/babelize-config
	$(chmodpath) 0755 ${babelizedir}/babelize
	$(chmodpath) 0755 ${babelizedir}/babelize-config
