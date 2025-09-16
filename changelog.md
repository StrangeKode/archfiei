<h2 align="center">ARCHFIEI : Cambios </h2>

### Julio 2025
- Se eliminó temporalmente el soporte para `btrfs` debido a un bug con grub+btrfs que deja el sistema instalado inbooteable 
- Se eliminó el soporte para `jfs` por bugs (sistema inbooteable)
- Perfil ISO actualizado a `archiso 84-1`
- Última base con nuevos paquetes
- Actualización de todos los paquetes de Archcraft y AUR
- Corregidos problemas con rofi
- Pequeñas mejoras y correcciones

#

### Abril 2025
- Perfil ISO actualizado a `archiso 83-1`
- Última base con nuevos paquetes
- Actualización de todos los paquetes de Archcraft y AUR
- Configuraciones de Openbox y Bspwm actualizadas
- Corregidos diseños del menú de rofi
- Corregidas caídas de Polybar
- Pequeñas mejoras y correcciones

#

### Enero 2025
- Perfil ISO actualizado a `archiso 82-1`
- Última base con nuevos paquetes
- Actualización de todos los paquetes de ARCHFIEI y AUR
- Pequeñas mejoras y correcciones

#

### Octubre 2024
- Perfil ISO actualizado
- Última base con nuevos paquetes
- Actualización de todos los paquetes de ARCHFIEI y AUR
- Añadidos nuevos temas de cursor, iconos y GTK (y actualizaciones a los existentes)
- Añadidos nuevos temas de openbox (y actualizaciones a los existentes)
- Añadidas nuevas tipografías e iconos nerd (y actualizaciones a los existentes)
- Actualizaciones de temas en ambos WMs (Polybar, Rofi, etc.)
- Añadidos 5 estilos/temas nuevos para openbox
- Añadidos 4 nuevos sets de iconos para el menú de openbox
- Añadido soporte para terminal `kitty` en ambos WMs
- Configuraciones de `alacritty` actualizadas
- Nueva configuración de `neofetch`
- Tema de `zsh` actualizado
- Nueva configuración de `picom`
- Varias correcciones y más

#

### Julio 2024
- Perfil ISO actualizado
- Última base con nuevos paquetes
- Actualización de todos los paquetes de Archcraft y AUR
- Actualización de configuraciones de Openbox
- Añadido Firewall (`ufw`) con GUI (`gufw`)
- Añadido `apparmor` para MAC (control de acceso obligatorio)
- Rofi reemplazado por el fork de ibonn, corregido el enfoque en compositores Wayland
- Pequeñas mejoras y correcciones

#

### Abril 2024
- Perfil ISO actualizado
- Última base con nuevos paquetes
- Actualización de todos los paquetes de Archcraft y AUR
- Actualización de todas las configuraciones de los WMs
- Añadido `calamares` con su configuración (corregido autologin)
- Añadido nuevo paquete de `grub` (corregida instalación en `xfs`)
- Añadidos hooks de grub (instalar grub en cada actualización)
- Añadido `archcraft-arandr` (GUI) para gestionar layouts de pantalla
- Corregido theming de QT, añadidos configs para QT6
- Mejoradas acciones de thunar (terminal, root, fondo de pantalla persistente)
- Pequeñas mejoras y correcciones

#

### Enero 2024
- Perfil ISO actualizado
- Última base con nuevos paquetes
- Actualización de todos los paquetes de ARCHFIEI y AUR
- Migración de `alacritty` a su nuevo formato (de `yml` a `toml`)
- Actualizados todos los scripts relacionados con alacritty
- Añadido módulo `tray` en polybar y corregidas fuentes
- Pequeñas mejoras y correcciones

#

### Octubre 2023
- Perfil ISO actualizado
- Última base con nuevos paquetes
- Añadida app `archcraft-randr` para gestionar pantallas/monitores
- WMs actualizados:
  - PKGBUILDs limpiados y código actualizado
  - Directorio `openbox-themes` fusionado en `openbox`; nueva estructura de configuración
  - Añadidos layouts de ejemplo multi-monitor en `bspwmrc` (uno, dos, tres monitores)
  - Soporte multi-monitor en todos los WMs (usa `archcraft-randr`)
- Añadida función `wipe` en ABIF
- Corregida la app de ayuda y tips
- Eliminado `python2`
- Pequeñas mejoras y correcciones

> Info: Ahora las actualizaciones de paquetes de WMs no reemplazan tus configs modificadas; se instalan en `~/.config/<nombre>_pacnew_<fecha>`. Puedes usar `meld` para fusionar cambios.

#

### Julio 2023
- Perfil ISO actualizado con el último archiso
- Última base con nuevos paquetes
- Corregido `xfce-power-manager` (bloqueo al cerrar tapa)
- Corregido SDDM no guardando la última sesión
- Añadida calculadora
- Openbox:
  - `tint2` como panel alternativo; cambio fácil entre paneles
  - Módulo y applet de bluetooth
  - Arreglado redimensionado por bordes
- BSPWM:
  - Módulo y applet de bluetooth
- Varias correcciones

#

### Abril 2023
Actualizaciones (1 mayo y 17 abril) con mejor soporte Nvidia, correcciones `pacman-init`, autologin y selector de escritorio en calamares. Además:
- ISO actualizada con últimos paquetes
- Activación de click único en rofi
- Corregidos módulos de volumen en polybar
- `picom` oficial; configs para forks disponibles (renombrar al que uses)
- Correcciones menores

#

### Enero 2023
Lanzamiento mayor con base reescrita desde cero: mejor soporte de red, bluetooth, audio (Pipewire), impresoras, códecs, gestores de archivos, multi-monitor, fuentes CJK, nuevos temas, etc. Se requiere reinstalar Archcraft para esta versión.

#

### Septiembre 2022
- ISO actualizada con últimos paquetes
- Corregidos menús/applet de Rofi
- Correcciones menores

#

### Julio 2022
- Base ISO según `archiso 65-1` (grub para UEFI)
- `zstd` para mkinitcpio
- Corregidos avisos de consola
- Config SDDM actualizada
- Usuarios/grupos actualizados
- Openbox como sesión por defecto en SDDM corregido
- Scripts y configs de WMs actualizados
- Nuevo BSPWM y nuevo motor de temas (temas infinitos)
- Modo fácil en openbox

#

### Junio 2022
- Corregido tema de plymouth
- Parámetros por defecto de kernel en grub mejorados
- Vuelve tema Slime
- ASCII de neofetch actualizado
- Paquetes actualizados

#

### Abril 2022
Limpieza grande: se removieron paquetes innecesarios; se actualizaron WMs; cambios menores en Openbox y BSPWM; eliminación de applets de red; arreglos en menús y dunst; mejoras en ABIF; configuración unificada de lockscreen; eliminación de scripts poco usados; sistema más limpio.

#

### Febrero 2022
No es major: configs de Alacritty, Dunst y WMs actualizadas; screenshots al portapapeles

#

### Octubre 2021
Bugfix para v21.09: drivers, flatpak/snap removidos, cambio a SDDM, mejoras en WMs y polybar

#

### Septiembre 2021
Reconstrucción desde cero: nueva base, logo, paquetes, repo; arreglos Nvidia, kernels; soporte snap/flatpak; Chaotic AUR; servicios habilitados; temas, apps, fuentes, estilos; grandes mejoras en configuraciones y herramientas CLI (vim, neovim, ranger, omz, ncmpcpp)

#

### Junio 2021
Autologin, sudo sin password en live, terminal extra, instaladores compatibles con copy-to-RAM, mejoras en pacman, polkit agent, acciones extra en thunar, correcciones y enlaces nuevos

#

### Mayo 2021
Calamares añadido, ABIF actualizado, base mejorada, `btrfs` por defecto, mejores snapshots, cambio a alacritty, soporte bluetooth/impresoras, más drivers gráficos, herramientas QT, nuevos temas, mejoras en bspwm, lockscreens por sesión, nuevos temas de plymouth/gtk/iconos/cursor, fuente actualizada a último archiso

#

### Abril 2021
Corregido blackscreen post login y otros bugs menores

#

### Enero 2021
Correcciones de tapa, congelamientos, layout HD, brillo, compositor, y nuevos launchers/powermenus

#

### Octubre 2020
Corregido powermenu, notificaciones duplicadas de mpd, tapping, VPN, módulo de red clicable, editor sin distracciones, más soporte Nvidia

#

### Septiembre 2020
Guía de inicio, nuevo look, soporte AMD/Nvidia, atajos familiares, plugins para HTML5, selector de estilos de lanzador/powermenu, fuentes corregidas, mejor menú de openbox, ecualizador de audio, script para detectar problemas comunes
