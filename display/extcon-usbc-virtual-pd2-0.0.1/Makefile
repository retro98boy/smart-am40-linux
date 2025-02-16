KERNEL_BUILD_DIR = /lib/modules/$(KERNELRELEASE)/build
PWD = $(shell pwd)

obj-m += extcon-usbc-virtual-pd2.o

modules:
	$(MAKE) -C $(KERNEL_BUILD_DIR) M=$(PWD) modules

clean:
	rm -rf $(shell ls -A | grep -v extcon-usbc-virtual-pd2.c | grep -v Makefile)

.PHONY: clean
