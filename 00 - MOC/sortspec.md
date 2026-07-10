---
orden: "99"
tags: [config, MOC]
sorting-spec: |
  target-folder: Weightlifting
  < a-z
  target-folder: Weightlifting/*
  < a-z by-metadata: orden
  target-folder: Weightlifting/05 - Tecnica
  /:files
   < a-z by-metadata: orden
  /folders
   Arranque
   Cargada
   Envion
  target-folder: Weightlifting/07 - Errores
  /:files
   < a-z by-metadata: orden
  /folders
   Tiron
   Arranque
   Cargada
   Envion
  target-folder: Weightlifting/08 - Ejercicios
  /:files
   < a-z by-metadata: orden
  /folders
   Arranque
   Cargada
   Envion
   Fuerza
   Accesorios
  target-folder: Weightlifting/09 - Programacion
  /:files
   < a-z by-metadata: orden
  /folders
   Adaptacion
   Variables
   Ciclos
  target-folder: Weightlifting/18 - Mi Practica
  /:files
   < a-z by-metadata: orden
  /folders
   Templates
   Bloques
   Sesiones
---

# ⚙️ sortspec — Orden Pedagógico del Vault

> [!warning] No borres ni renombres esta nota
> El nombre del archivo **debe ser `sortspec`** — es el único nombre que el plugin **Custom File Explorer sorting** reconoce para leer la configuración. El bloque `sorting-spec` del frontmatter de arriba controla el orden de lectura de todo el vault.

## Cómo funciona

Cada nota tiene un campo `orden:` en su frontmatter (`"01"`, `"02"`, …) que fija su posición pedagógica dentro de su carpeta. Esta spec le dice a Obsidian:

1. **`Weightlifting`** → las carpetas se ordenan por nombre (`00 → 99`).
2. **`Weightlifting/*`** (todas las subcarpetas) → las notas se ordenan por el valor de su campo `orden`.
3. **Carpetas con subcarpetas** (05 Técnica, 07 Errores, 08 Ejercicios, 09 Programación, 18 Mi Práctica) → primero las notas sueltas (por `orden`), luego las subcarpetas en secuencia pedagógica (p. ej. Arranque → Cargada → Envión).

> Las rutas llevan el prefijo `Weightlifting/` porque la raíz del vault de Obsidian es la carpeta *Obsidian Vault*, y *Weightlifting* es una subcarpeta.

## Activación

Tras crear o editar esta nota, **hacé clic en el icono del plugin en la barra lateral** (o ejecutá el comando **`sort-on`** desde la paleta `Ctrl+P`) para que el plugin relea y aplique la spec. El estado se recuerda entre sesiones.

## Reordenar una nota

Cambiá el número en su campo `orden:`. Mantené siempre 2 dígitos (`"01"`, no `"1"`) para que el orden alfabético coincida con el numérico. Una nota nueva sin `orden:` cae al final de su carpeta.
