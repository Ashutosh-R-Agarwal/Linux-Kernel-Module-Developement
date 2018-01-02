obj-m += hello.o

ifndef KERNEL_MBUILD_SOURCE
        KERNEL_MBUILD_SOURCE=/lib/modules/$(shell uname -r)/build
endif

all:
	make -C $(KERNEL_MBUILD_SOURCE) M=$(PWD) modules

clean:
	make -C $(KERNEL_MBUILD_SOURCE) M=$(PWD) clean

