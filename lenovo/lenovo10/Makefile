.PHONY: install uninstall set-default

uninstall:
	rm -rv /usr/share/plymouth/themes/lenovo10 || true

install: uninstall
	mkdir /usr/share/plymouth/themes/lenovo10
	cp -v *.script *.plymouth *.png /usr/share/plymouth/themes/lenovo10/

set-default:
	plymouth-set-default-theme -R lenovo10
