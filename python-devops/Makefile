#!/usr/bin/make -f

install:
	install -d											$(DESTDIR)/usr/bin
	install -d											$(DESTDIR)/usr/share/pyshared
	install -m755	$(CURDIR)/src/devops/bin/dos.py		$(DESTDIR)/usr/bin/
	cp -r 			$(CURDIR)/src/devops/devops			$(DESTDIR)/usr/share/pyshared/
