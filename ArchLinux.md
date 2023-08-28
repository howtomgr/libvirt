# Archlinux virt server

## Install packages

```shell
sudo pacman -S libvirt iptables-nft dnsmasq bridge-utils virt-manager virt-viewer swtpm qemu
```

## Remove iptables

```shell
sudo pacman -R iptables 
```

## Enable services

```shell
sudo systemctl enable libvirtd virtnetworkd
```

## Add user to libvirt group

```shell
sudo usermod -a -G libvirt $USER
```

