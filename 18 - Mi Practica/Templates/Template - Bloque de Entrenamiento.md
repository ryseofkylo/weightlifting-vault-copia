---
orden: "02"
tags: [template, práctica-personal]
---

# Bloque de Entrenamiento — {{nombre del bloque}}

**Período:** {{fecha inicio}} → {{fecha fin}}  
**Semanas:** ___  
**Fase:** Preparatoria / Precompetitiva / Competitiva  
**Sesiones/semana:** ___  
**Macrociclo:** ___ | **Mesociclo:** ___ | **Microciclo inicio:** ___

---

## Marcas Personales (usadas para calcular %)

> ⚠️ Estos PRs NO cambian durante todo el macrociclo — incluso si hacés un nuevo PR en la semana 9

| Lift | PR (kg) |
|---|---|
| Arranque | |
| Cargada & Envión | |
| Front Squat | |
| Back Squat | |

---

## Objetivos del Bloque

**Técnicos:**
- 

**De fuerza:**
- 

**De volumen total planificado:**
- Total reps del bloque: ___
- Intensidad media objetivo: ___%

---

## Punto de Control Planificado

**Fecha del test:** {{fecha}}  
**Semana:** ___  
**Objetivo arranque:** ___ kg  
**Objetivo C&J:** ___ kg

---

## Estructura Semanal

| Semana | Volumen (reps) | Intensidad promedio | Zona principal | Notas |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |
| 6 | | | | |
| 7 (test) | | | 100% | |
| 8 | | | | |
| 9 (test) | | | 100%+ | |
| 10 | | | | |
| 11 | | | | |
| 12 (comp) | | | MAX | |

---

## Ejercicios Planificados

### Lifts Primarios
- Arranque
- Cargada & Envión

### Fuerza
- Front Squat / Back Squat
- Pulls

### Técnicos
- _______________

### Accesorio
- _______________

---

## Revisión al Final del Bloque

**¿Llegué a los objetivos?**  
- Arranque: Esperado ___ kg / Logrado ___ kg  
- C&J: Esperado ___ kg / Logrado ___ kg  

**¿% de lifts fallidos mayor al 10% en alguna semana?**  
- Semana ___: ___% → ¿Qué acción se tomó?

**Qué funcionó:**  
- 

**Qué cambiaría en el próximo bloque:**  
- 

**Errores técnicos recurrentes del bloque:**  
- → Ver [[MOC - Errores y Corrección]]

---

## Sesiones del Bloque

```dataview
TABLE date, bodyweight, lifts
FROM "Mi Practica/Sesiones"
WHERE bloque = "{{nombre del bloque}}"
SORT date ASC
```
