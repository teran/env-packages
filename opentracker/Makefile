#!/usr/bin/make -f

pre-build:
	cvs -d :pserver:anoncvs@cvs.erdgeist.org:/home/cvsroot co opentracker
	$(MAKE) -C opentracker -f Makefile

clean:
	rm -rvf opentracker

install:
	install -d												$(DESTDIR)/usr/bin
	install -d												$(DESTDIR)/usr/share/pyshared
	install -m755	$(CURDIR)/src/opentracker/opentracker	$(DESTDIR)/usr/bin/
	install -m644	$(CURDIR)/src/opentracker.conf			$(DESTDIR)/etc/
