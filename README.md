![logo](https://edteam-media.s3.amazonaws.com/blogs/big/2ab53939-9b50-47dd-b56e-38d4ba3cc0f0.png)

# Herramientas de Escaneo de Red

## :information_source: Descripción
"Findips_arp-scan" y "Findips_nmap" son herramientas implementadas en scripts Bash que utilizan arp-scan y nmap respectivamente. Estas herramientas son útiles para detectar direcciones IP activas en la red, ofreciendo una forma rápida y sencilla de obtener información sobre los dispositivos conectados. Se recomienda ejecutar ambos scripts con privilegios de superusuario para acceder a todas las funciones de escaneo de red disponibles.

## :arrow_down: Instalacion
```bash
cd /opt
sudo rm -rf Findips
sudo git clone https://github.com/JennValentine/Findips.git
sudo chmod +x Findips/*
cd Findips
ls -lthas
```

## :book: Acceso directo
```bash
cd 
sudo echo "cd /opt/Findips/ && sudo ./Findips_arp-scan" > Findips_arp-scan
sudo echo "cd /opt/Findips/ && sudo ./Findips_nmap" > Findips_nmap
sudo chmod +x Findips_arp-scan
sudo chmod +x Findips_nmap
sudo rm -rf /usr/local/bin/Findips_arp-scan
sudo rm -rf /usr/local/bin/Findips_nmap
sudo mv Findips_arp-scan /usr/local/bin/
sudo mv Findips_nmap /usr/local/bin/
cd
```

## :book: Archivos ieee-oui.txt y mac-vendor.txt para Findips_arp-scan
```bash
sudo cp /usr/share/arp-scan/ieee-oui.txt /opt/Findips
sudo cp /etc/arp-scan/mac-vendor.txt /opt/Findips
```

## :hammer: Modo de Uso

Ejecutar el script en la red:

Herramienta 1: Escaneo de IP's Activas en la red (ARP-SCAN)

```bash
sudo Findips_arp-scan
```
![logo](https://github.com/JennValentine/Findips/blob/main/Imagenes/Findips_arp-scan.jpg)
:books: DATA: 
* Obtiene la dirección IP y la dirección MAC de la interfaz de red.
* Obtiene el rango de red.
* Utiliza arp-scan para escanear las direcciones IP dentro del rango de red en busca de dispositivos activos.
* Filtra y muestra solo las direcciones IP activas encontradas en la red.

Herramienta 2: Escaneo de IP's Activas en la red (NMAP)

```bash
sudo Findips_nmap
```
![logo](https://github.com/JennValentine/Findips/blob/main/Imagenes/Findips_nmap.jpg)
:books: DATA: 

* Obtiene la dirección IP y la dirección MAC de la interfaz de red.
* Obtiene el rango de red.
* Utiliza Nmap para escanear las direcciones IP dentro del rango de red en busca de dispositivos activos.
* Filtra y muestra solo las direcciones IP activas encontradas en la red.

:bookmark_tabs: En resumen, ambas script automatiza el proceso de encontrar direcciones IP activas en una red.

## :octocat: Créditos
1. [Jenn Valentine](https://t.me/JennValentine) - Update Contributor
