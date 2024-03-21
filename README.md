![logo](https://edteam-media.s3.amazonaws.com/blogs/big/2ab53939-9b50-47dd-b56e-38d4ba3cc0f0.png)

# Herramientas de Escaneo de Red

## Descripción

Este conjunto de scripts Bash se encarga de buscar direcciones IP activas en la red local 
utilizando diferentes métodos de escaneo. Ambas herramientas ofrecen una forma rápida y sencilla 
de identificar dispositivos activos en la red y proporcionan información útil sobre la 
configuración de red del sistema local.

## :book: Instalacion
```bash
cd /opt
sudo rm -rf Findips
sudo git clone https://github.com/JennValentine/Findips.git
sudo chmod +x Findips/*
cd Ping-TTL
```

## :book: Acceso directo
```bash
sudo cp Findips_arp-scan Findips_arp-scan_$RANDOM.sh
sudo cp Findips_nmap Findips_nmap_$RANDOM.sh
sudo rm -rf /usr/local/bin/Findips_arp-scan
sudo rm -rf /usr/local/bin/Findips_nmap
sudo mv Findips_arp-scan /usr/local/bin/
sudo mv Findips_nmap /usr/local/bin/
cd
```

## Modo de Uso

Ejecutar el script en la red local:


```bash
sudo Findips_arp-scan
```
* Herramienta 1: Escaneo de IP's Activas en la red local (ARP-SCAN)

Este script utiliza ARP-SCAN para buscar direcciones IP activas en la red local.

```bash
sudo Findips_nmap
```
* Herramienta 2: Escaneo de IP's Activas en la red local (NMAP)

Este script utiliza NMAP para buscar direcciones IP activas en la red local.

DATA: Ambas herramientas proporcionan una forma rápida y eficiente de escanear direcciones IP activas en la red local. 
Es importante ejecutar los scripts con permisos de superusuario para acceder a la funcionalidad de escaneo de red.

## :octocat: Créditos
1. [Jenn Valentine](https://t.me/JennValentine) - Update Contributor
