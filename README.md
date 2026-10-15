# Sistema de Registro de Asistencia - Pollería

Prototipo funcional para el desafío del curso Fundamentos de Programación (CIIN1205P).
Registra la asistencia del personal de una pollería organizado en 2 turnos (Mañana y
Tarde), calcula las horas trabajadas y exporta un resumen MENSUAL con el pago de cada
trabajador a un archivo Excel.

## Estructura del proyecto

```
main.py                    Programa principal (menú de consola)
modulo_validaciones.py     Validación de código, nombre, turno, fecha y hora
modulo_Empleados.py     Registro y búsqueda de trabajadores
modulo_asistencia.py       Registro de entrada/salida y cálculo de horas
modulo_persistencia.py     Guardado y lectura de datos en archivos de texto
modulo_reportes.py         Resumen mensual, cálculo de pago y exportación a Excel
modulo_planilla.py    Resuelve la regla de negocio, el pago al personal es mensual y depende de las horas trabajadas.    
test_pruebas.py            Casos de prueba con datos simulados de campo
data/                       Carpeta donde se guardan los archivos .txt y .xlsx
```


