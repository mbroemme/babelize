# The top-level input Makefile for mpq-tools

# minimum required automake 1.6
AUTOMAKE_OPTIONS = 1.6

# architecture-independent data files
babelizedir = $(datadir)/babelize
langpackdir = $(datadir)/babelize/langpacks
babelize_DATA = babelize

EXTRA_DIST = $(babelize_DATA)

install-data-hook:
	$(sedpath) 's,@BASH@,${bashpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@BASENAME@,${basenamepath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@CP@,${cppath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@RM@,${rmpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@MV@,${mvpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@CHMOD@,${chmodpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@GREP@,${greppath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@SED@,${sedpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@MKDIR@,${mkdirpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@FIND@,${findpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@MD5SUM@,${md5sumpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@TAR@,${tarpath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@XDELTA@,${xdeltapath},g' -i ${babelizedir}/babelize
	$(sedpath) 's,@STAT@,${statpath},g' -i ${babelizedir}/babelize
	$(mkdirpath) -p ${langpackdir}
