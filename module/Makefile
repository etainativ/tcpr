obj-m += tcpr.o
tcpr-y := module.o filter.o
ccflags-y := -O1 -ggdb3 -I$(src)/../include

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) modules

install:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) modules_install

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) clean
