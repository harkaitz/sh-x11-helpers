PROJECT=sh-x11-helpers
VERSION=1.0.0
DESTDIR =
PREFIX  =/usr/local


all:
clean:
install:
update:

## -- BLOCK:license --
install: install-license
install-license: 
	mkdir -p $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
	cp LICENSE README.md $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT)
update: update-license
update-license:
	ssnip README.md
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-exec      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-todo           $(DESTDIR)$(PREFIX)/bin
	cp bin/dmenu-fsel       $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-open      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-report         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-trans     $(DESTDIR)$(PREFIX)/bin
	cp bin/x-wiki           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-monitor        $(DESTDIR)$(PREFIX)/bin
	cp bin/x-editor         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-auto           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-edit      $(DESTDIR)$(PREFIX)/bin
	cp bin/x-open           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-postit         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-pipe      $(DESTDIR)$(PREFIX)/bin
	cp bin/xdg-pipe         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-clip-clean     $(DESTDIR)$(PREFIX)/bin
	cp bin/x-menu           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-note           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-link           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-color          $(DESTDIR)$(PREFIX)/bin
	cp bin/x-screenshot     $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
