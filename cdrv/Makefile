obj-m := chrdrv_skel.o
#obj-m += chrdrv_dyn.o
obj-m += chrdrv_udev.o
obj-m += chrdrv_reg.o
obj-m += chrdrv_misc.o

KDIR = /lib/modules/$(shell uname -r)/build
PWD = $(shell pwd)

all:
	$(MAKE) -C $(KDIR) M=$(PWD) modules
clean:
	@rm -rf a.out
	$(MAKE) -C $(KDIR) M=$(PWD) clean
