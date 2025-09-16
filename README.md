# ARCHFIEI : Perfil ISO 

### ¿Qué es?
- Perfil personalizado de ArchISO para generar la ISO de ARCHFIEI.
- Incluye lista de paquetes, configuración de arranque (UEFI/BIOS), y scripts de personalización del sistema live/instalado.

### Estructura clave
- `profile/profiledef.sh`: Metadatos y modos de arranque de la ISO.
- `profile/packages.x86_64`: Paquetes instalados en el live.
- `profile/bootstrap_packages.x86_64`: Paquetes mínimos para bootstrap.
- `profile/mkarchcraftiso`: Script de construcción (derivado de mkarchiso).
- `profile/airootfs/`: Archivos copiados dentro del rootfs del live.
- `profile/airootfs/root/customize_airootfs.sh`: Ajustes finales dentro del chroot del live.
- `profile/pacman.conf`: Configuración de pacman para la build.
- `profile/efiboot/loader/*`: Entradas systemd-boot.
- `profile/grub/*.cfg`: Menús GRUB.
- `profile/syslinux/*.cfg`: Config para BIOS/pxe.

### Requisitos del host
- Paquetes: archiso, dosfstools, mtools, squashfs-tools, xorriso, grub (para modos GRUB).

### Cómo construir
```bash
cd archfiei-master
./profile/mkarchcraftiso -v profile/
```

### Personalización rápida
- Cambia nombre/label/modos en `profile/profiledef.sh`.
- Agrega o quita paquetes en `profile/packages.x86_64`.
- Ajusta repos en `profile/pacman.conf`.
- Edita tweaks del sistema en `profile/airootfs/root/customize_airootfs.sh`.
