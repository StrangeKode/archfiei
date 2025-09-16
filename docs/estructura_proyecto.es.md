# Estructura del proyecto 

Este documento describe cada parte del perfil ISO y dónde modificar para personalizar la build.

## Raíz del repositorio
- `README.md` / `README.es.md`: Descripción del proyecto.
- `changelog.md` / `changelog.es.md`: Historial de cambios.
- `profile/`: Perfil ArchISO.

## `profile/`
- `profiledef.sh`: Metadatos y opciones de build
  - `iso_name`, `iso_label`, `iso_version`, `install_dir`.
  - `buildmodes`, `bootmodes` (BIOS/UEFI, GRUB/systemd-boot).
  - `airootfs_image_type` y opciones de compresión.
  - `file_permissions`: permisos aplicados tras copiar `airootfs`.
- `packages.x86_64`: Lista de paquetes del live.
- `bootstrap_packages.x86_64`: Lista mínima para modo bootstrap.
- `pacman.conf`: Repos y opciones de pacman durante la build.
- `mkarchcraftiso`: Script de construcción (instala paquetes, prepara bootloaders, empaqueta ISO).

## `profile/airootfs/`
Contenido que se copia al rootfs del live.
- `etc/*`: Configs del sistema (locale, mkinitcpio, network, systemd, polkit, sudoers, X11, etc).
- `root/customize_airootfs.sh`: Script que corre dentro del chroot para ajustes finales (mkinitcpio, repos, zsh por defecto, apparmor, copiar dotfiles de `skel`, autostart, ocultar .desktop, etc).
- `usr/local/bin/*`: Scripts utilitarios como `choose-mirror`.

## Bootloaders
- `efiboot/loader/*`: systemd-boot (UEFI), entradas con kernel args por defecto.
- `grub/*.cfg`: Menús GRUB para Default/OpenSource/Nvidia/Nomodeset.
- `syslinux/*.cfg`: Configs para BIOS/pxe.

## Dónde personalizar
- Nombre/versión/etiqueta ISO: `profiledef.sh`.
- Paquetes: `packages.x86_64`.
- Repos: `pacman.conf`.
- Ajustes live/iniciales: `airootfs/root/customize_airootfs.sh` y `airootfs/etc/*`.
- Opciones de arranque: `grub/*.cfg`, `efiboot/loader/entries/*.conf`, `syslinux/*.cfg`.

## Build
- Requisitos: `archiso`, `dosfstools`, `mtools`, `squashfs-tools`, `xorriso`, `grub` (si usas GRUB).
- Comando: `sudo /home/arc/Escritorio/archfiei/profile/mkarchcraftiso /home/arc/Escritorio/archfiei/profile`.
