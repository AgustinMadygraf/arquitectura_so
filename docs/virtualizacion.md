# Bloque especifico: Virtualizacion

## Objetivo

Entender que es virtualizar, que tipos existen y como se relaciona con WSL2 en este curso.

## 1) Conceptos base

- Virtualizacion: ejecutar sistemas aislados sobre el mismo hardware fisico.
- Host: sistema operativo base de la maquina.
- Guest: sistema operativo invitado dentro de una VM.
- Hipervisor: capa que administra VMs y recursos.

## 2) Tipos de hipervisor

- Tipo 1 (bare-metal): corre directo sobre hardware.
- Tipo 2 (hosted): corre sobre un SO host.

## 3) Virtualizacion vs contenedores

- VM: virtualiza hardware + kernel propio por guest.
- Contenedor: comparte kernel del host, aísla procesos/FS/red.
- En general, VM tiene mayor aislamiento; contenedor mayor eficiencia.

## 4) WSL2 en el contexto del curso

- WSL2 usa virtualizacion liviana para correr kernel Linux en Windows.
- Permite ejecutar practicas Bash/Python de SO desde entorno Linux real.
- Ver guia operativa: `docs/guia_wsl2.md`.

## 5) Practica guiada minima

### Parte A (Windows PowerShell)

```powershell
wsl --status
wsl -l -v
```

Preguntas:
1. ¿La version predeterminada es 2?
2. ¿La distro activa esta en VERSION 2?

### Parte B (dentro de WSL)

```bash
uname -a
cat /proc/version
```

Preguntas:
1. ¿Que kernel informa el sistema?
2. ¿Ves referencia a Microsoft/WSL en la salida?

## 6) Criterio de logro

Se considera logrado cuando el estudiante:
- explica diferencias VM vs contenedor,
- identifica tipo de virtualizacion usada por WSL2,
- verifica por comandos que su entorno esta operativo.
