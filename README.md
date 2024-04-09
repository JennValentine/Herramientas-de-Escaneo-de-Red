![logo](https://edteam-media.s3.amazonaws.com/blogs/big/2ab53939-9b50-47dd-b56e-38d4ba3cc0f0.png)

# Herramientas de Escaneo de Red

## :information_source: DescripciÛn
Este conjunto de scripts Bash se encarga de buscar direcciones IP activas en la red local 
utilizando diferentes m√©todos de escaneo. Ambas herramientas ofrecen una forma r√°pida y sencilla 
de identificar dispositivos activos en la red y proporcionan informaci√≥n √∫til sobre la 
configuraci√≥n de red del sistema local.

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
cd /opt/Findips
sudo cp Findips_arp-scan Findips_arp-scan_$RANDOM
sudo rm -rf /usr/local/bin/Findips_arp-scan
sudo mv Findips_arp-scan /usr/local/bin/
sudo cp Findips_nmap Findips_nmap_$RANDOM
sudo rm -rf /usr/local/bin/Findips_nmap
sudo mv Findips_nmap /usr/local/bin/
cd
```

## :hammer: Modo de Uso

Ejecutar el script en la red local:

Herramienta 1: Escaneo de IP's Activas en la red local (ARP-SCAN)

```bash
sudo Findips_arp-scan
```
![logo](https://github.com/JennValentine/Findips/blob/main/Imagenes/Findips_arp-scan.jpg)
:books: DATA: Este script utiliza ARP-SCAN para buscar direcciones IP activas en la red local.


Herramienta 2: Escaneo de IP's Activas en la red local (NMAP)

```bash
sudo Findips_nmap
```
![logo](https://github.com/JennValentine/Findips/blob/main/Imagenes/Findips_nmap.jpg)
:books: DATA: Este script utiliza NMAP para buscar direcciones IP activas en la red local.

:bookmark_tabs: Ambas herramientas proporcionan una forma r·pida y eficiente de escanear direcciones IP activas en la red local.
Es importante ejecutar los scripts con permisos de superusuario para acceder a la funcionalidad de escaneo de red.

## :octocat: CrÈditos
1. [Jenn Valentine](https://t.me/JennValentine) - Update Contributor
