#	arm-linux-ld -Ttext 0x0000000 -g demokey.o -o demokey_elf
demokey.bin : demokey.S
	arm-linux-gcc -g -c -o demokey.o $<
	arm-linux-ld -Tmyld.lds -g demokey.o -o demokey_elf
	arm-linux-objcopy -O binary -S demokey_elf $@
clean :
	rm -f demokey.bin demokey_elf *.o
