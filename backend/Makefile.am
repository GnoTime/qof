
if EMBEDDED
XML=
SQLITE=sqlite
else
if USE_SQLITE
SQLITE=sqlite
else
SQLITE=
endif
XML=file
endif

SUBDIRS = $(XML) $(SQLITE)

DIST_SUBDIRS = file sqlite
