<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 2


<!-- Su documentación aquí -->
Ejercicios con bucle while:
Solicita al usuario que ingrese una lista de números y encuentra el número mayor y el menor.
Solicita al usuario un número e imprime la suma de los números pares entre 1 y ese número.
Solicita al usuario una cadena e imprime cuántas vocales contiene.
Solicita al usuario un número y muestra su tabla de potencias desde 1 hasta 10.
Solicita al usuario una lista de números y calcula la media aritmética.
```python

numbers = list(map(int, input("Ingrese una lista de números separados por espacio: ").split()))
max_num = max(numbers)
min_num = min(numbers)
print("Número mayor:", max_num)
print("Número menor:", min_num)

# ... (Resto de los ejercicios con bucle while)

# Después de cada ejercicio, realiza el commit de los cambios:
git add archivo.py  # Reemplaza "archivo.py" con el nombre de tu archivo Python
git commit -m "Resuelto ejercicio de bucle while: Encuentra el número mayor y menor"

```

Ejercicios con bucle for:
Solicita al usuario una lista de números y calcula la suma de sus elementos.
Solicita al usuario una lista de números e imprime cuántos de ellos son pares.
Solicita al usuario un número y muestra su tabla de multiplicar usando range().
Solicita al usuario un número e imprime los números pares desde 2 hasta ese número.
Solicita al usuario un número y muestra la secuencia de números pares desde 2 hasta ese número.
```python
# Solicita al usuario una lista de números y calcula la suma de sus elementos.
numbers = list(map(int, input("Ingrese una lista de números separados por espacio: ").split()))
sum_elements = sum(numbers)
print("Suma de los elementos:", sum_elements)

# ... (Resto de los ejercicios con bucle for)

# Después de cada ejercicio, realiza el commit de los cambios:
git add archivo.py  # Reemplaza "archivo.py" con el nombre de tu archivo Python
git commit -m "Resuelto ejercicio de bucle for: Calcula la suma de los elementos"

```

Acciones en el repositorio local:

Captura de pantalla de la configuración inicial del repositorio.
Hacer commit por cada ejercicio.
Captura de pantalla del comando git log.
Captura de pantalla del comando git diff.
```python
git init
git add captura_configuracion.png
git commit -m "Agrega captura de pantalla de configuración inicial del repositorio"

git add captura_git_log.png
git commit -m "Agrega captura de pantalla del comando git log"

git add captura_git_diff.png
git commit -m "Agrega captura de pantalla del comando git diff"
```






