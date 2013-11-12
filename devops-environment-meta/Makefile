#!/usr/bin/make -f

install:
	install -d											$(DESTDIR)/etc/libvirt
	install -m644 $(CURDIR)/src/libvirt/libvirtd.conf   $(DESTDIR)/etc/libvirt/
	install -d											$(DESTDIR)/etc/default
	install -m644 $(CURDIR)/src/libvirt/libvirt-bin	$(DESTDIR)/etc/default/

