THISDIR = $(shell pwd)
xray_URL := https://raw.githubusercontent.com/hiboyhiboy/opt-file/master/v2ray

all:download_xray

download_xray: 
	curl --create-dirs -L $(xray_URL) -o $(THISDIR)/bin/xray
	
clean: 
	rm -rf $(THISDIR)/bin
	
romfs:
	$(ROMFSINST) -p +x $(THISDIR)/bin/xray /usr/bin/v2ray