.PHONY: install uninstall set-default

uninstall:
	rm -rv /usr/share/plymouth/themes/lg10 || true

install: uninstall
	mkdir /usr/share/plymouth/themes/lg10
	cp -v *.script *.plymouth *.png /usr/share/plymouth/themes/lg10/

set-default:
	plymouth-set-default-theme -R lg10
