.PHONY: install uninstall set-default

uninstall:
	rm -rv /usr/share/plymouth/themes/asus10 || true

install: uninstall
	mkdir /usr/share/plymouth/themes/asus10
	cp -v *.script *.plymouth *.png /usr/share/plymouth/themes/asus10/

set-default:
	plymouth-set-default-theme -R asus10
