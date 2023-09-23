<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 1 


<!-- Su documentación aquí -->
¿Cuál es tu nivel de conocimiento de Python? (principiante, intermedio, avanzado) Explica brevemente.
R/principiante
¿Has usado Git/GitHub antes? ¿Con qué frecuencia? (nunca, una o dos veces, varias veces)
R/nunca
¿Has escrito código en Python? ¿De qué tipo? (algoritmos simples, funciones, clases, librerías, proyectos completos)
R/no
```python
import math

# Definir una clase llamada "Circulo" que representa un círculo
class Circulo:
    def __init__(self, radio):
        self.radio = radio

    def calcular_area(self):
        return math.pi * self.radio ** 2

    def calcular_perimetro(self):
        return 2 * math.pi * self.radio 

# Función para calcular el diámetro de un círculo dado su radio
def calcular_diametro(radio):
    return 2 * radio

# Crear una instancia de la clase Circulo
mi_circulo = Circulo(5)

# Calcular el área y el perímetro del círculo usando métodos de la clase
area = mi_circulo.calcular_area()
perimetro = mi_circulo.calcular_perimetro()

# Calcular el diámetro del círculo usando la función
diametro = calcular_diametro(mi_circulo.radio)

# Imprimir los resultados
print(f"Área del círculo: {area}")
print(f"Perímetro del círculo: {perimetro}")
print(f"Diámetro del círculo: {diametro}")

import math

# Definir una clase llamada "Circulo" que representa un círculo
class Circulo:
    def __init__(self, radio):
        self.radio = radio

    def calcular_area(self):
        return math.pi * self.radio ** 2

    def calcular_perimetro(self):
        return 2 * math.pi * self.radio

# Función para calcular el diámetro de un círculo dado su radio
def calcular_diametro(radio):
    return 2 * radio

# Crear una instancia de la clase Circulo
mi_circulo = Circulo(5)

# Calcular el área y el perímetro del círculo usando métodos de la clase
area = mi_circulo.calcular_area()
perimetro = mi_circulo.calcular_perimetro()

# Calcular el diámetro del círculo usando la función
diametro = calcular_diametro(mi_circulo.radio)

# Imprimir los resultados
print(f"Área del círculo: {area}")
print(f"Perímetro del círculo: {perimetro}")
print(f"Diámetro del círculo: {diametro}") 
```

Python
https://www.canva.com/design/DAFtPyOPdu8/cA90_USDfphP_BDqEXlY7g/edit?utm_content=DAFtPyOPdu8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
git
https://www.canva.com/design/DAFtQCAxPJM/uSVarf5BzK36Pr8DKH9_kA/edit?utm_content=DAFtQCAxPJM&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
github 
https://www.canva.com/design/DAFtQEBJ8x8/7NEqxZRvjt03YAOtWhgy0g/edit?utm_content=DAFtQEBJ8x8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton




