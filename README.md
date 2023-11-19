# Jarkom-Modul-3-I10-2023

Praktikum Jaringan Komputer Modul 3 I10
Computer Network Practicum 3rd Module I10

| Name                        | NRP        |
|-----------------------------|------------|
|Riski Ilyas                  | 5025211189 |
|Vija Wildan Gita Prabawa     | 5025211261 |

## Number 1
Lakukan konfigurasi sesuai dengan peta yang sudah diberikan.

### Topology
![topology](https://media.discordapp.net/attachments/919468862725046322/1175793363295932416/image.png?ex=656c85e6&is=655a10e6&hm=5de6b7b5c44229befe4c01d825434e343bffd321acad019298bb9424184d278c&=&width=956&height=702)

### Config

- Aura
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.233.3.9
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.233.4.9
	netmask 255.255.255.0

auto eth3
iface eth3 inet static
	address 192.233.1.9
	netmask 255.255.255.0

auto eth4
iface eth4 inet static
	address 192.233.2.9
	netmask 255.255.255.0

```

- Himmel
```auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.233.3.9
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 192.233.4.9
	netmask 255.255.255.0

auto eth3
iface eth3 inet static
	address 192.233.1.9
	netmask 255.255.255.0

auto eth4
iface eth4 inet static
	address 192.233.2.9
	netmask 255.255.255.0
```

- Heiter
```
auto eth0
iface eth0 inet static
	address 192.233.1.2
	netmask 255.255.255.0
	gateway 192.233.1.9
```

- Denken
```
auto eth0
iface eth0 inet static
	address 192.233.2.3
	netmask 255.255.255.0
	gateway 192.233.2.9
```

- Elsen
```
auto eth0
iface eth0 inet static
	address 192.233.2.2
	netmask 255.255.255.0
	gateway 192.233.2.9
```

- Revolte
```
auto eth0
iface eth0 inet dhcp
        hwaddress ether 12:23:34:45:56:67
```

- Richter
```
auto eth0
iface eth0 inet dhcp
        hwaddress ether 12:34:56:78:9A:BC
```

- Lawine
```
auto eth0
iface eth0 inet static
	address 192.233.3.1
	netmask 255.255.255.0
	gateway 192.233.3.9
```

- Linie
```
auto eth0
iface eth0 inet static
	address 192.233.3.2
	netmask 255.255.255.0
	gateway 192.233.3.9
```

- Lugner
```
auto eth0
iface eth0 inet static
	address 192.233.3.3
	netmask 255.255.255.0
	gateway 192.233.3.9
```

- Sein
```
auto eth0
iface eth0 inet dhcp
        hwaddress ether AA:BB:CC:DD:EE:FF
```

- Stark
```
auto eth0
iface eth0 inet dhcp
        hwaddress ether 1A:2B:3C:4D:5E:6F
```

- Frieren
```
auto eth0
iface eth0 inet static
	address 192.233.4.1
	netmask 255.255.255.0
	gateway 192.233.4.9
```

- Flamme
```
auto eth0
iface eth0 inet static
	address 192.233.4.2
	netmask 255.255.255.0
	gateway 192.233.4.9
```

- Fern
```
auto eth0
iface eth0 inet static
	address 192.233.4.3
	netmask 255.255.255.0
	gateway 192.233.4.9
```
