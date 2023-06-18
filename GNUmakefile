DESTDIR =
PREFIX  =/usr/local


all:
clean:
install:
update:
## -- install-sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/x-color          $(DESTDIR)$(PREFIX)/bin
	cp bin/x-screenshot     $(DESTDIR)$(PREFIX)/bin
## -- install-sh --
## -- license --
install: install-license
install-license: LICENSE
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/sh-x11-helpers
	cp LICENSE $(DESTDIR)$(PREFIX)/share/doc/sh-x11-helpers
## -- license --
