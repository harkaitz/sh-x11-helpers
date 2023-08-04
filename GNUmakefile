PROJECT=sh-x11-helpers
VERSION=1.0.0
DESTDIR =
PREFIX  =/usr/local


all:
clean:
install:
update:

## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-exec      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-phone          $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-trans     $(DESTDIR)$(PREFIX)/bin
	cp bin/x-record         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-auto           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-edit      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-pipe      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-color          $(DESTDIR)$(PREFIX)/bin
	cp bin/x-screenshot     $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE README.md $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
update: update-license
update-license:
	ssnip README.md
## -- BLOCK:license --
