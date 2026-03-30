# SO_AC

Este repositorio acompana la materia **Sistemas Operativos y Arquitectura de Computadoras**.
Si sos estudiante, usalo como guia de practica paso a paso.

## Como vamos a trabajar

- Vamos a aprender haciendo.
- Cada microleccion es corta y ejecutable.
- Primero entendemos el comportamiento del sistema, despues subimos dificultad.

## Trayectos del curso

1. Python (laboratorio de conceptos de SO/Arquitectura)
2. Bash (comandos y automatizacion en Linux/WSL2)
3. PowerShell (comandos y automatizacion en entorno Microsoft)

## Entorno de trabajo

- Python y Bash: **WSL2 (Linux)**.
- PowerShell: PowerShell 7+.
- Sin GUI y sin frameworks.

## Trayecto Python: librerias y herramientas

Estandar:
- `pathlib`
- `os`
- `subprocess`
- `platform`
- `shutil`
- `mmap`
- `socket`
- `signal`
- `resource`

Externa:
- `psutil` (instalada con `pip`)

Herramienta operativa:
- `venv` (entorno virtual)

## Orden didactico del trayecto Python

1. `pathlib`
2. `os`
3. `subprocess`
4. `platform`
5. `shutil`
6. `venv`
7. `psutil`
8. `mmap`
9. `socket`
10. `signal`
11. `resource` (al final)

## Estructura

- `microlecciones/python/`: carpetas `NN_libreria/` con scripts `.py`.
- `microlecciones/bash/`: practicas `.sh`.
- `microlecciones/powershell/`: practicas `.ps1`.
- `docs/`: guias y plan.

## Ejecucion (ejemplo)

```bash
python3 microlecciones/python/01_pathlib/01_intro_pathlib.py
```

## Documentacion

- `docs/plan_microlecciones.md`
- `docs/metodologia.md`
- `docs/estructura.md`
- `docs/todo.md`
