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
	install -D -t $(DESTDIR)$(PREFIX)/share/doc/$(PROJECT) LICENSE
## -- BLOCK:license --
## -- BLOCK:sh --
install: install-sh
install-sh:
	mkdir -p $(DESTDIR)$(PREFIX)/bin
	cp bin/x-pipe           $(DESTDIR)$(PREFIX)/bin
	cp bin/txt-open         $(DESTDIR)$(PREFIX)/bin
	cp bin/txt-edit         $(DESTDIR)$(PREFIX)/bin
	cp bin/txt-save-link    $(DESTDIR)$(PREFIX)/bin
	cp bin/x-editor         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-open           $(DESTDIR)$(PREFIX)/bin
	cp bin/txt-exec         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-menu           $(DESTDIR)$(PREFIX)/bin
	cp bin/x-search         $(DESTDIR)$(PREFIX)/bin
	cp bin/x-link           $(DESTDIR)$(PREFIX)/bin
	cp bin/txt-search       $(DESTDIR)$(PREFIX)/bin
	cp bin/x-compat         $(DESTDIR)$(PREFIX)/bin
## -- BLOCK:sh --
