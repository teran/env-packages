#!/usr/bin/make -f

SRCDIR='src/opentracker'

build:
	cvs -d :pserver:anoncvs@cvs.erdgeist.org:/home/cvsroot co "${SRCDIR}"
	cd "${SRCDIR}"
	make
	cd ../..

clean:
	rm -rvf "${SRCDIR}"

install:
	install -d												$(DESTDIR)/usr/bin
	install -d												$(DESTDIR)/usr/share/pyshared
	install -m755	$(CURDIR)/${SRCDIR}/opentracker			$(DESTDIR)/usr/bin/
	install -m644	$(CURDIR)/$(SRCDIR)/opentracker.conf	$(DESTDIR)/etc/
