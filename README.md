# Actividad-Diagnostica-Rompe-C-digo
Primera actividad y diagrama de flujo de algoritmos y estructura de datos
# Actividad Diagnóstica: Rompe-código

Repositorio con la solución a los 3 retos de lógica y algoritmos de la actividad inicial.

---

## Reto 1: Reto de los Vasos

**Objetivo:** Intercambiar el agua (Vaso B) y el jugo (Vaso A) usando un tercer vaso vacío (Vaso C).

### Pasos:
1. Verter el jugo del vaso A dentro del vaso C. *(A queda vacío)*.
2. Pasamos el agua del vaso B al vaso A. *(B queda vacío)*.
3. Pasamos el jugo del vaso C al vaso B. *(C vuelve a quedar vacío)*.


## Reto 2: Reto Triage

**Objetivo:** Determinar la prioridad de atención médica (Alta, Media, Baja) de un paciente.

### Reglas de decisión:
* **Alta:** Si el paciente presenta una urgencia.
* **Media:** Si no es urgencia, pero el paciente tiene 65 años o más, O lleva esperando 60 minutos o más.
* **Baja:** Si no cumple ninguna de las condiciones anteriores.

### Ejemplos probados:
* **Paciente 1 (70 años, Urgencia: No, Espera: 30 min):** Prioridad **Media** (por la edad).
* **Paciente 2 (28 años, Urgencia: Sí, Espera: 10 min):** Prioridad **Alta** (por la urgencia).
* **Paciente 3 (35 años, Urgencia: No, Espera: 120 min):** Prioridad **Media** (por el tiempo de espera).


## Reto 3: Reto del Adivino

**Objetivo:** Adivinar un número entre 1 y 100 en un máximo de 7 intentos.

### Estrategia (Búsqueda a la mitad / Binaria):
1. Definir el rango inicial de búsqueda entre 1 y 100.
2. Preguntar siempre por el número que está en el punto medio del rango actual.
3. Según la respuesta:
   * **"Es mayor":** Se descarta la mitad inferior. El nuevo límite mínimo es el número dicho + 1.
   * **"Es menor":** Se descarta la mitad superior. El nuevo límite máximo es el número dicho - 1.
   * **"¡Correcto!":** Se termina el juego.

4. Repetir el proceso con el nuevo rango. 

Al ir dividiendo las opciones a la mitad en cada paso (100 -> 50 -> 25 -> 12 -> 6 -> 3 -> 1), se garantiza adivinar el número en 7 intentos o menos.
