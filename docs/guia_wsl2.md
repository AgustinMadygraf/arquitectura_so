# Guia operativa WSL2 (instalacion, verificacion y version)

## Objetivo

Disponer de un entorno Linux (WSL2) para ejecutar las practicas de Python y Bash.

## Requisito

- Windows 10/11 con permisos de administrador.

## Instalacion inicial (PowerShell como administrador)

```powershell
wsl --install
```

Luego:
1. Reinicia el equipo cuando lo solicite Windows.
2. Abre la distribucion instalada (por ejemplo, Ubuntu) y crea usuario/contrasena.

## Verificacion rapida

```powershell
wsl --status
```

Esperado:
- WSL habilitado.
- Version predeterminada en 2.

## Listado de distribuciones y version

```powershell
wsl -l -v
```

Esperado:
- Cada distro con su estado y version.
- La columna VERSION debe indicar 2 para usar WSL2.

## Convertir una distro de WSL1 a WSL2

```powershell
wsl --set-version <DistroName> 2
```

Ejemplo:

```powershell
wsl --set-version Ubuntu 2
```

## Definir WSL2 como predeterminado

```powershell
wsl --set-default-version 2
```

## Ver version de componentes WSL

```powershell
wsl --version
```

## Prueba minima desde Linux (dentro de WSL)

```bash
uname -r
python3 --version
```

## Problemas comunes

- Si `wsl --install` falla, verifica que la virtualizacion este habilitada en BIOS/UEFI.
- Si una distro queda en VERSION 1, ejecuta `wsl --set-version <DistroName> 2`.
- Si no abre ninguna distro, reinstala desde Microsoft Store y repite `wsl -l -v`.
