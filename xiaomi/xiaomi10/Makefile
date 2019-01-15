.PHONY: install uninstall set-default

uninstall:
	rm -rv /usr/share/plymouth/themes/xiaomi10 || true

install: uninstall
	mkdir /usr/share/plymouth/themes/xiaomi10
	cp -v *.script *.plymouth *.png /usr/share/plymouth/themes/xiaomi10/

set-default:
	plymouth-set-default-theme -R xiaomi10
