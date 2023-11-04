<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


<!-- Su documentación aquí -->
```python

data = {
    "centro_atencion": ["UH SANTA CRUZ", "UH DOCE DE OCTUBRE", "UH MANRIQUE", "CS TRINIDAD", "UH CASTILLA", 
                        "UH SAN CRISTOBAL", "UH NUEVO OCCIDENTE", "CS ROBLEDO", "CS SANTO DOMINGO", 
                        "CS CISAMF", "UH BELEN", "CS LORETO", "CS ESTADIO", "CS SAN LORENZO", 
                        "CS MANANTIAL DE VIDA", "CS POPULAR", "CS ARANJUEZ", "CS EL SALVADOR", 
                        "CS GUAYABAL", "CS SANTA ROSA DE LIMA", "CS MORAVIA", "CS PABLO VI", 
                        "CS LIMONAR", "CS BELEN ALTAVISTA", "UH SAN JAVIER", "CS PICACHITO", 
                        "CS CARPINELO", "CS SANTA ELENA", "CS EL RAIZAL", "CS ENCISO", "CS CIVITON", 
                        "CS SOL DE ORIENTE", "CS BELEN RINCON"],
    "direccion": ["Carrera 51A # 100 - 80", "Calle 101BB # 78 - 10", "Calle 66E # 42 - 51", 
                  "Calle 27 Â # Â 65D - 49", "Carrera 65 # 98 - 115", "Calle 62D # 133 - 15", 
                  "Carrera 102C # 63B - 65", "Calle 75 # 75-29", "Carrera 33 # 107B â€“15", 
                  "Carrea 51D No. 71 - 02", "Calle 28 # 77-124", "Carrera 28A  # 38F - 84", 
                  "Calle 48 # 73 - 10", "Cll. 41 No. 42A-68", "Calle 57F # 92CC - 107", 
                  "Carrera 43B # 108 - 6", "Carrera 50A # 93-39", "Cra 36 #  40A-30", 
                  "Calle 9 Sur # 52 - 42", "Calle 49DD # 87 - 11", "Carrera 55  # 79B - 29", 
                  "Calle 120 # 50 - 11", "Carrera 63 # 49B Sur - 7", "Calle 18 # 105 -15", 
                  "Calle 40 # 105 - 103", "Carrera 83B  # 97AA - 82", "Calle 97A   # 24F - 90", 
                  "Km 16", "Carrera 32  # 71A â€“ 51", "Carrera 29A # 59-31", "Calle 77C  # 91 - 65", 
                  "Carrera 17B # 56EE - 89", "Calle 2B # 79 -100"],
    "comuna": ["SANTA CRUZ", "DOCE DE OCTUBRE", "MANRIQUE", "GUAYABAL", "CASTILLA", 
               "SAN CRISTOBAL", "SAN CRISTOBAL", "ROBLEDO", "POPULAR", "ARANJUEZ", 
               "BELEN", "BUENOS AIRES", "LAURELES", "LA CANDELARIA", "SAN JAVIER", 
               "POPULAR", "ARANJUEZ", "BUENOS AIRES", "GUAYABAL", "SAN JAVIER", 
               "ARANJUEZ", "SANTA CRUZ", "SAN ANTONIO DE PRADO", "ALTAVISTA", "SAN JAVIER", 
               "DOCE DE OCTUBRE", "POPULAR", "SANTA ELENA", "MANRIQUE", "VILLA HERMOSA", 
               "ROBLEDO", "VILLA HERMOSA", "BELEN"],
    "barrio": ["Santa Cruz", "Doce de Octubre No.2", "Manrique Oriental", "Trinidad", 
               "Castilla", "Cabecera Urbana San Cristobal", "Ãrea de ExpansiÃ³n Pajarito", 
               "La Pilarica", "Santo Domingo Savio No. 1", "Sevilla", "BelÃ©n", "Loreto", 
               "El Estadio", "Las Palmas", "Blanquizal", "Popular", "San Isidro", "Gerona", 
               "La Colina", "Los AlcÃ¡zares", "Moravia", "Pablo VI", "Cabecera San Antonio de Prado", 
               "Altavista Sector Central", "Veinte de Julio", "Picacho", "Aldea Pablo VI", 
               "Santa Elena Sector Central", "Versalles No. 1", "Enciso", "Aures No.1", 
               "Trece de Noviembre", "El RincÃ³n"],
    "Longitud": [-75.56057776, -75.57883982, -75.55309557, -75.58650566, -75.56938634, 
                 -75.63824853, -75.61294191, -75.58814331, -75.54283567, -75.56476096, 
                 -75.5983006, -75.55586179, -75.5915023, -75.56611511, -75.60580946, 
                 -75.54920505, -75.55874111, -75.56060339, -75.58899173, -75.60574263, 
                 -75.56605542, -75.55297355, -75.64307775, -75.62730101, -75.62038033, 
                 -75.58320655, -75.54142142, -75.49742845, -75.54481229, -75.55008797, 
                 -75.59309304, -75.5405399, -75.60370365],
    "Latitud": [6.29348089, 6.302168039, 6.262030262, 6.228777905, 6.293090342, 6.278332361, 
                6.2824425, 6.276309524, 6.294609693, 6.267868575, 6.228853799, 6.233197481, 
                6.254417702, 6.240071745, 6.274513173, 6.297297606, 6.285118826, 6.237965021, 
                6.201086673, 6.262403258, 6.274741428, 6.304349318, 6.17546016, 6.222967586, 
                6.254340806, 6.297484169, 6.286665184, 6.209558753, 6.26680911, 6.250639883, 
                6.243545336, 6.212329777]
}

# Crear el DataFrame
df = pd.DataFrame(data)

# Filtro 1: usando una condición booleana (por ejemplo, seleccionar centros de atención en la comuna 'SANTA CRUZ')
filtro_condicion_booleana = df[df['comuna'] == 'SANTA CRUZ']

# Filtro 2: usando una función de selección (por ejemplo, seleccionar centros de atención con Longitud menor a -75.6)
filtro_longitud_menor = df[df['Longitud'] < -75.6]

# Filtro 3: usando una función de selección (por ejemplo, seleccionar centros de atención con Longitud mayor a -75.6)
filtro_longitud_mayor = df[df['Longitud'] > -75.6]

# Filtro 4: usando una función de selección (por ejemplo, seleccionar centros de atención con Latitud menor a 6.25)
filtro_latitud_menor = df[df['Latitud'] < 6.25]

# Filtro 5: usando una función de selección (por ejemplo, seleccionar centros de atención con Latitud mayor a 6.25)
filtro_latitud_mayor = df[df['Latitud'] > 6.25]

# Filtro 6: Todas las filas donde la "direccion" es menor que la calle 50
filtro_menor_calle_50 = df[df["direccion"].apply(lambda x: int(x.split()[0]) if x.split()[0].isdigit() else None) < 50]

# Filtro 7: Todas las filas donde la "direccion" es mayor que la calle 50
filtro_mayor_calle_50 = df[df["direccion"].apply(lambda x: int(x.split()[0]) if x.split()[0].isdigit() else None) > 50]


# Filtrar 8: el DataFrame utilizando las palabras clave
palabras_clave = ["UH SANTA CRUZ", "UH DOCE DE OCTUBRE", "CS PABLO VI"]
filtro_palabras_clave = df[df['centro atención'].isin(palabras_clave)]


# Imprimir los resultados
print("Filtro usando una condición booleana:")
print(filtro_condicion_booleana)

print("\nFiltro usando una función de selección para Longitud menor a -75.6:")
print(filtro_longitud_menor)

print("\nFiltro usando una función de selección para Longitud mayor a -75.6:")
print(filtro_longitud_mayor)

print("\nFiltro usando una función de selección para Latitud menor a 6.25:")
print(filtro_latitud_menor)

print("\nFiltro usando una función de selección para Latitud mayor a 6.25:")
print(filtro_latitud_mayor)

print("Filtradas todas las filas donde la 'direccion' es menor que la calle 50:")
print(filtro_menor_calle_50)

print("\nFiltradas todas las filas donde la 'direccion' es mayor que la calle 50:")
print(filtro_mayor_calle_50)

print("Filtradas las filas con palabras clave:")
print(filtro_palabras_clave)



