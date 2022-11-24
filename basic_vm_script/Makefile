PREFIX?=/usr/local
BINDIR=$(DESTDIR)$(PREFIX)/bin

INSTALL=/usr/bin/install
MKDIR=/bin/mkdir

SCRIPT=samplevm

install:
	$(MKDIR) -p $(BINDIR)
	$(INSTALL) -m 544 $(SCRIPT) $(BINDIR)/
