# Sistema de Registro de Asistencia - Pollería

Prototipo funcional para el desafío del curso Fundamentos de Programación (CIIN1205P).
Registra la asistencia del personal de una pollería organizado en 2 turnos (Mañana y
Tarde), calcula las horas trabajadas y exporta un resumen MENSUAL con el pago de cada
trabajador a un archivo Excel.

## Estructura del proyecto

```
main.py                    Programa principal (menú de consola)
modulo_validaciones.py     Validación de código, nombre, turno, fecha y hora
modulo_trabajadores.py     Registro y búsqueda de trabajadores
modulo_asistencia.py       Registro de entrada/salida y cálculo de horas
modulo_persistencia.py     Guardado y lectura de datos en archivos de texto
modulo_reportes.py         Resumen mensual, cálculo de pago y exportación a Excel
test_pruebas.py            Casos de prueba con datos simulados de campo
diagrama.py                Genera el diagrama de flujo (diagrama_flujo.png)
data/                       Carpeta donde se guardan los archivos .txt y .xlsx
```

## Requisitos

```
pip install openpyxl
```

## Cómo ejecutar

```
python main.py          # Programa interactivo con menú
python test_pruebas.py  # Corre casos de prueba automáticos
```

## Notas

- El turno Tarde puede cruzar la medianoche; el cálculo de horas lo maneja
  automáticamente `calcular_horas_trabajadas()` en `modulo_asistencia.py`.
- La tarifa por hora (`TARIFA_HORA` en `main.py`) es referencial: ajústala al
  acuerdo real con el dueño del negocio.
- Antes de la entrega, sube este proyecto a un repositorio en GitHub con
  commits progresivos (ver sugerencia de historial en el informe técnico,
  Paso 5).
