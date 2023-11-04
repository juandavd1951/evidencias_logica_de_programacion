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





