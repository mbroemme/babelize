# The top-level input Makefile for mpq-tools

# minimum required automake 1.6
AUTOMAKE_OPTIONS = 1.6

# architecture-independent data files
babelizedir = $(datadir)/babelize
langpackdir = $(datadir)/babelize/langpacks
babelize_DATA = babelize

EXTRA_DIST = $(babelize_DATA)

install-data-hook:
	$(sedpath) 's,@BASH@,${bashpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@BASENAME@,${basenamepath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@CP@,${cppath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@RM@,${rmpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@MV@,${mvpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@CHMOD@,${chmodpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@GREP@,${greppath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@SED@,${sedpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@MKDIR@,${mkdirpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@FIND@,${findpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@MD5SUM@,${md5sumpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@TAR@,${tarpath},' -i ${babelizedir}/babelize
	$(sedpath) 's,@XDELTA@,${xdeltapath},' -i ${babelizedir}/babelize
	$(mkdirpath) -p ${langpackdir}
