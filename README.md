# uboot
port_uboot contains steps on how to port uboot

step 1
make lewis2440_config
make

patch with following command:
patch -p0 --ignore-whitespace --no-backup-if-mismatch < patch_turnoff_led_jump.patc
