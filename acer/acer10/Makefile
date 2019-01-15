.PHONY: install uninstall set-default

uninstall:
	rm -rv /usr/share/plymouth/themes/acer10 || true

install: uninstall
	mkdir /usr/share/plymouth/themes/acer10
	cp -v *.script *.plymouth *.png /usr/share/plymouth/themes/acer10/

set-default:
	plymouth-set-default-theme -R acer10
