#!/usr/bin/make -f

pre-build:
	cvs -d :pserver:anoncvs@cvs.erdgeist.org:/home/cvsroot co opentracker
	$(MAKE) -C opentracker -f Makefile

clean:
	rm -rvf $(CURDIR)/opentracker

install:
	install -d												$(DESTDIR)/usr/bin
	install -d												$(DESTDIR)/usr/share/pyshared
	install -d												$(DESTDIR)/etc/ubic/service
	install -m755	$(CURDIR)/opentracker/opentracker		$(DESTDIR)/usr/bin/opentracker
	install -m644	$(CURDIR)/src/opentracker.conf			$(DESTDIR)/etc/opentracker.conf
	install -m644	$(CURDIR)/src/ubic.service				$(DESTDIR)/etc/ubic/service/opentracker
