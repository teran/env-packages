#!/usr/bin/make -f

build:
	rm -rvf src/seed
	git clone git://github.com/teran/seed.git src/seed

clean:
	dh_clean
	rm -rvf src/seed

install:
	install -d											$(DESTDIR)/usr/share/python-django-seed
	install -d											$(DESTDIR)/etc/uwsgi/apps-available
	install -d											$(DESTDIR)/etc/uwsgi/apps-enabled
	install -m644	$(CURDIR)/src/seed.yaml				$(DESTDIR)/etc/uwsgi/apps-available/seed.yaml
	cp -r 			$(CURDIR)/src/seed					$(DESTDIR)/usr/share/python-django-seed/

