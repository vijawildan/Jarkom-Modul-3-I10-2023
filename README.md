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

## Soal 2
Client yang melalui Switch3 mendapatkan range IP dari [prefix IP].3.16 - [prefix IP].3.32 dan [prefix IP].3.64 - [prefix IP].3.80

### Answer
```
echo 'subnet 192.233.1.0 netmask 255.255.255.0 {
}
 
subnet 192.233.2.0 netmask 255.255.255.0 {
}
 
subnet 192.233.3.0 netmask 255.255.255.0 {
	range 192.233.3.16 192.233.3.32;
	range 192.233.3.64 192.233.3.80;
	option routers 192.233.3.0;
}'
```

## Soal 3
Client yang melalui Switch4 mendapatkan range IP dari [prefix IP].4.12 - [prefix IP].4.20 dan [prefix IP].4.160 - [prefix IP].4.168 (3)

### Answer
```
echo 'subnet 192.233.1.0 netmask 255.255.255.0 {
}
 
subnet 192.233.2.0 netmask 255.255.255.0 {
}
 
subnet 192.173.3.0 netmask 255.255.255.0 {
	range 192.173.3.16 192.173.3.32;
	range 192.173.3.64 192.173.3.80;
	option routers 192.173.3.0;
}
 
subnet 192.233.4.0 netmask 255.255.255.0 {
	range 192.233.4.12 192.173.4.20;
	range 192.233.4.160 192.173.4.168;
	option routers 192.173.4.0;
} '
```

## Soal 4
Client mendapatkan DNS dari Heiter dan dapat terhubung dengan internet melalui DNS tersebut

### Answer
![4a](https://media.discordapp.net/attachments/919468862725046322/1175805979976290375/image.png?ex=656c91a7&is=655a1ca7&hm=d012719e155e73f6e6fec0ae62fd8fa5047d107416805bec14a06eafa12459bb&=&width=1175&height=481)
![4b](https://media.discordapp.net/attachments/919468862725046322/1175806192841408582/image.png?ex=656c91d9&is=655a1cd9&hm=4a9f6b38c0d1f3def9a97c9592728c23a93df839e14496d23f99e0b9ea76ec26&=&width=1175&height=476)
![4c](https://media.discordapp.net/attachments/919468862725046322/1175806314736263228/image.png?ex=656c91f6&is=655a1cf6&hm=947ed9ee357c713da534cd7b11d62eb7f67bbdc81c06a45e44020e202c7ee12d&=&width=1175&height=596)
![4d](https://media.discordapp.net/attachments/919468862725046322/1175806376128282674/image.png?ex=656c9205&is=655a1d05&hm=3dafdbc3cb78b1939481cb6425fa9c17ef4cff9464144f434695410dd938cbd4&=&width=1175&height=622)

## Soal 5
Lama waktu DHCP server meminjamkan alamat IP kepada Client yang melalui Switch3 selama 3 menit sedangkan pada client yang melalui Switch4 selama 12 menit. Dengan waktu maksimal dialokasikan untuk peminjaman alamat IP selama 96 menit

### Answer
![5a](https://cdn.discordapp.com/attachments/919468862725046322/1175806846360105071/image.png?ex=656c9275&is=655a1d75&hm=a2ec64d7405fa166cf743d0d74a99f8bcd69076a5ec1e565bfbdc4d0c12ffc3f&)

## Soal 6
Pada masing-masing worker PHP, lakukan konfigurasi virtual host untuk website berikut dengan menggunakan php 7.3.

### Answer
![6a](https://media.discordapp.net/attachments/919468862725046322/1175807369381421077/image.png?ex=656c92f2&is=655a1df2&hm=e0f273ba0f6f8bc5c8e24d32be0c49d43de0e5498273e5050f633110c08e6d40&=&width=1175&height=672)
![6b](https://media.discordapp.net/attachments/919468862725046322/1175807456971067562/image.png?ex=656c9307&is=655a1e07&hm=4817eed8c3ec3052465f556fa2621169103f0f539d114fa21550b137cfb62993&=&width=1175&height=656)

## Soal 12
Selanjutnya LB ini hanya boleh diakses oleh client dengan IP [Prefix IP].3.69, [Prefix IP].3.70, [Prefix IP].4.167, dan [Prefix IP].4.168. (12) hint: (fixed in dulu clinetnya)

### Answer
![12a](https://media.discordapp.net/attachments/919468862725046322/1175807661678276690/image.png?ex=656c9337&is=655a1e37&hm=ee93d2cef37a2a0b5bbfc6d188ddef97f9803e20af47de36dab7659ba960925e&=&width=1175&height=697)
