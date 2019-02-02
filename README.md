# Flexplexico Configuration Management

## Network Structure

TODO


## Manual Setup

### GRUB Bootloader

Due to the lack of AMD drivers, the `nomodeset` parameter must be passed to the
kernel upon startup. Modify the contents of `/etc/default/grub` such that
`GRUB_CMDLINE_LINUX="nomodeset"`, save the file, and run `update-grub`.


### Sudo

```
apt-get -y install sudo
echo "patrick ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/patrick
```


### Python

`apt-get -y install python`


### Add SSH Public Key

`ssh-copy-id 192.168.1.122`
