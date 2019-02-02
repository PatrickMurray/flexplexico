# Flexplexico Configuration Management

## Network Structure



## Manual Setup

### GRUB Bootloader

Due to the lack of AMD drivers, the `nomodeset` parameter must be passed to the
kernel upon startup. Modify the contents of `/etc/default/grub` such that
`GRUB_CMDLINE_LINUX="nomodeset"`, save the file, and run `update-grub`.


### Add SSH Public Key

`ssh-copy-id 192.168.1.122`
