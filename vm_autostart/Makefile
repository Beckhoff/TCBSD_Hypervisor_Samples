PREFIX?=/usr/local
BINDIR=$(DESTDIR)$(PREFIX)/bin
RCDIR=$(DESTDIR)$(PREFIX)/etc/rc.d

INSTALL=/usr/bin/install
MKDIR=/bin/mkdir

SCRIPT=samplevm

install:
	$(MKDIR) -p $(BINDIR)
	$(INSTALL) -m 544 $(SCRIPT) $(BINDIR)/

	$(MKDIR) -p $(RCDIR)
	$(INSTALL) -m 555 rc.d/* $(RCDIR)/
