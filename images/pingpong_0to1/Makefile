# Automatically generated with gzll-image-create, do not edit

SCRIPTDIR=$(shell pkg-config --variable=buildscriptdir optimsoc-gzll)

all: image.elf image.bin image.vmem

APP_BINARY_OBJECTS = pingpong_sender_binary.o pingpong_receiver_binary.o 
pingpong_sender.bin: ../../apps/pingpong/sender.elf
	or1k-elf-objcopy -O binary $^ $@
pingpong_receiver.bin: ../../apps/pingpong/receiver.elf
	or1k-elf-objcopy -O binary $^ $@
include $(SCRIPTDIR)/Makefile-images.inc
