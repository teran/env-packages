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
	install	-d											$(DESTDIR)/etc/nginx/sites-available
	install -d											$(DESTDIR)/etc/nginx/sites-enabled
	install -m644	$(CURDIR)/src/uwsgi.yaml			$(DESTDIR)/etc/uwsgi/apps-available/seed.yaml
	install -m644	$(CURDIR)/src/nginx.conf			$(DESTDIR)/etc/nginx/sites-available/seed.conf
	cp -r 			$(CURDIR)/src/seed					$(DESTDIR)/usr/share/python-django-seed/

