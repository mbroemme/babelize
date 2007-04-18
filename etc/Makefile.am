# The top-level input Makefile for mpq-tools

# minimum required automake 1.6
AUTOMAKE_OPTIONS = 1.6

# architecture-independent sysconf files
sysconf_DATA = babelize.conf

install-data-hook: babelize.conf
	$(sedpath) 's,LANGPACK_DIR=.*,LANGPACK_DIR="$(datadir)/babelize/langpacks",' -i $(sysconfdir)/babelize.conf
