VER=01


BINPROGS = \
	easy-creds


install:

	install -dm755 $(DESTDIR)/usr/bin
	install -dm755 $(DESTDIR)/usr/share/easy-creds
	install -m755 $(BINPROGS) $(DESTDIR)/usr/bin
	install -m755 definitions.sslstrip $(DESTDIR)/usr/share/easy-creds

uninstall:
	for f in $(BINPROGS); do $(RM) $(DESTDIR)/usr/bin/$$f; done
	rm -rf $(DESTDIR)/usr/share/easy-creds


.PHONY: install uninstall
