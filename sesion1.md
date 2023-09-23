<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 1 


<!-- Su documentación aquí -->
- ¿Cuál es tu nivel de conocimiento de Python? (principiante, intermedio, avanzado) Explica brevemente.

- R/principiante

- ¿Has usado Git/GitHub antes? ¿Con qué frecuencia? (nunca, una o dos veces, varias veces)
- R/nunca
- ¿Has escrito código en Python? ¿De qué tipo? (algoritmos simples, funciones, clases, librerías, proyectos completos)
- R/no
- Escribe un breve ejemplo de código Python que involucre al menos dos de los siguientes conceptos: funciones, clases, librerías.

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
- Escribe los comandos de Git que conoces y una breve explicación de cada uno.

- R/no conozco ninguno pero estos son algunos

Git clone
Git clone es un comando para descargarte el código fuente existente desde un repositorio remoto (como Github, por ejemplo). En otras palabras, Git clone básicamente realiza una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en tu ordenador.
Hay un par de formas de descargar el código fuente, pero principalmente yo prefiero clonar de la forma con https:
git clone <https://link-con-nombre-del-repositorio>

Git branch
Las ramas (branch) son altamente importantes en el mundo de Git. Usando ramas, varios desarrolladores pueden trabajar en paralelo en el mismo proyecto simultáneamente. Podemos usar el comando git branch para crearlas, listarlas y eliminarlas.
Creando una nueva rama:
git branch <nombre-de-la-rama>
Este comando creará una rama en local. Para enviar (push) la nueva rama al repositorio remoto, necesitarás usar el siguiente comando:
git push <nombre-remoto> <nombre-rama>
Visualización de ramas:
git branch
git branch --list
Borrar una rama:
git branch -d <nombre-de-la-rama>
Comparten los resultados en el grupo y generan una lista de:
Conceptos de Python que deben reforzar
Comandos de Git que conocen la mayoría
Comandos de Git que deben aprender
Temas de Python que deben aprender
Ejemplos de código que deben escribir como práctica

- Actividad: Consulta y creación de infografía para cada tema: Python, Git y GitHub (Trabajo grupal)
Objetivo: Aprender los conceptos básicos de Python, Git y GitHub y crear una infografía para cada tema que explique de manera clara y visual.
Instrucciones:
Investiga sobre Python, Git y GitHub por separado. Busca información sobre qué son, para qué se utilizan y cuáles son sus principales características.
Selecciona la información más relevante y útil para crear una infografía para cada tema que explique de manera clara y visual los conceptos básicos de Python, Git y GitHub.
Utiliza herramientas de diseño gráfico para crear las infografías.

- Python
https://www.canva.com/design/DAFtPyOPdu8/cA90_USDfphP_BDqEXlY7g/edit?utm_content=DAFtPyOPdu8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
- git
https://www.canva.com/design/DAFtQCAxPJM/uSVarf5BzK36Pr8DKH9_kA/edit?utm_content=DAFtQCAxPJM&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
- github 
https://www.canva.com/design/DAFtQEBJ8x8/7NEqxZRvjt03YAOtWhgy0g/edit?utm_content=DAFtQEBJ8x8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton




