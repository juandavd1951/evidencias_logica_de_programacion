<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 


<!-- Su documentación aquí -->
Actividad: Ejercicio de limpieza de datos con Pandas
Crear un proyecto de Python y utilizar la librería pandas para realizar la limpieza de datos del siguiente conjunto de datos de venta de vehículos
Descargar - Conjunto de Datos "Venta de Vehiculos"
Documentar los problemas de datos encontrados

solulucion
```python

import pandas as pd

data = {
    "Fecha": ["2022-01-01", "2022-01-02", "2022-01-03", "2022-01-04", "2022-01-05", 
              "2022-01-06", "2022-01-07", "2022-01-08", "2022-01-09"],
    "Marca": ["Toyota", "Chevrolet", "Ford", "Toyota", "Chevrolet", "Chevrolet", 
              "Chevrolet", "Chevrolet", "Ford"],
    "Modelo": ["Sedán", "Sedán", "Camioneta", "SUV", "SUV", "Camioneta", "Camioneta", 
               "SUV", "Sedán"],
    "Año": [2016, 1997, 2021, 2009, 2012, 2015, 2006, 2014, 2001],
    "Precio": [32328.0, 16117.0, None, 20130.0, 17623.0, 26444.0, 34600.0, 22448.0, 13436.0],
    "Kilometraje": [3073, 78772, 72752, 48628, 31403, 23922, 18332, 150000, 19888],
    "Color": ["Rojo", "Azul", "Blanco", "Blanco", "Rojo", "Plateado", "Plateado", 
              "Plateado", "Azul"],
    "Estado": ["Usado", "Usado", "Usado", "Nuevo", "Usado", "Nuevo", "Nuevo", "Nuevo", "Nuevo"],
    "Descuento": [0, 0, 5, 0, 5, 15, 10, 15, 5],
    "Vendido": [False, False, True, False, False, True, True, False, False]
}

df = pd.DataFrame(data)

df.isna()

df = df.dropna()

print(df)
```
Documentación de Problemas de Datos:
1. Codificación de Caracteres:
Problema: Los datos contienen caracteres especiales como "Ã±" en lugar de "ñ" y "Ã¡" en lugar de "á".
Solución: Se requiere una corrección en la codificación de caracteres para mostrar los datos correctamente.
2. Datos Faltantes:
Problema: Algunos campos importantes tienen valores faltantes. Por ejemplo, el precio de la camioneta Ford en el tercer registro y el año del modelo de la camioneta Ford en el mismo registro.
Solución: Puedes decidir llenar los valores faltantes con datos predeterminados o eliminar las filas con datos incompletos, dependiendo del contexto y la importancia de los registros.
3. Tipos de Datos Incorrectos:
Problema: El campo "Año" está representado como cadena de texto en lugar de tipo numérico, lo que dificulta las operaciones matemáticas.
Solución: Convertir el campo "Año" a tipo numérico para realizar cálculos matemáticos.
4. Formato de Fecha Incorrecto:
Problema: El campo "Fecha" está en formato de texto. Para realizar análisis temporal, sería más útil si estuviera en formato de fecha.
Solución: Convertir el campo "Fecha" al formato de fecha adecuado para facilitar las operaciones de análisis temporal.
5. Descuentos y Precio Inconsistentes:
Problema: Algunos vehículos tienen descuentos, pero el precio no parece estar ajustado en consecuencia.
Solución: Verificar la consistencia de los datos y ajustar los precios de acuerdo con los descuentos, o asegurarse de que los descuentos estén correctamente aplicados.
6. Valores No Válidos en el Campo "Vendido":
Problema: El campo "Vendido" tiene valores booleanos, pero hay registros donde el valor es "False" (cadena de texto) en lugar de False (booleano).
Solución: Convertir los valores del campo "Vendido" a tipo booleano para garantizar la coherencia y facilitar futuros análisis.
7. Inconsistencia en el Campo "Estado":
Problema: Algunos vehículos están etiquetados como "Usado" y "Nuevo" en el campo "Estado", lo que puede ser contradictorio.
Solución: Verificar la coherencia de los datos y, si es necesario, estandarizar la terminología para el campo "Estado".





