<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->
Actividad: Resolver utilizando funciones en Python
Calculadora Básica: Crea una función llamada calculadora que tome tres argumentos: dos números y un operador (+, -, *, /). La función debe realizar la operación indicada en los dos números y devolver el resultado.
```python
def calculadora(num1, num2, operador):
    if operador == '+':
        return num1 + num2
    elif operador == '-':
        return num1 - num2
    elif operador == '*':
        return num1 * num2
    elif operador == '/':
        if num2 != 0:  # Verificar que el divisor no sea cero
            return num1 / num2
        else:
            return "Error: División por cero no permitida"

resultado = calculadora(5, 3, '+')  
print(resultado)
```

Conteo de Vocales: Crea una función llamada contar_vocales que tome una cadena como argumento y devuelva el número de vocales (a, e, i, o, u) que contiene la cadena.
Ejemplo de uso:
```python
def contar_vocales(cadena):
    cadena = cadena.lower()
   
    contador = 0
    
    for caracter in cadena:
    
        if caracter in "aeiou":
            contador += 1
    
    return contador

num_vocales = contar_vocales("Hola, mundo!")  
print(num_vocales)

```


Primo o No Primo: Escribe una función llamada es_primo que tome un número entero positivo como argumento y determine si es un número primo (es decir, solo es divisible por 1 y por sí mismo). La función debe devolver True si es primo y False si no lo es.
```python
def es_primo(numero):

    if numero <= 1:
        return False

    for i in range(2, int(numero**0.5) + 1):
        if numero % i == 0:
            return False

    return True


resultado = es_primo(2)  
print(resultado)
```

Contador de Palabras: Escribe una función llamada contar_palabras que tome una cadena como argumento y devuelva el número de palabras en esa cadena. Supón que las palabras están separadas por espacios.
```python
def contar_palabras(cadena):

    palabras = cadena.split()

    return len(palabras)


num_palabras = contar_palabras("Hola, este es un ejemplo. ")
print(num_palabras)  
```


Cálculo de Potencia: Escribe una función llamada potencia que tome dos números enteros como argumentos, uno como base y otro como exponente, y devuelva el resultado de elevar la base al exponente.

```python
def potencia(base, exponente):
 
    resultado = base ** exponente
    return resultado


resultado = potencia(2, 2)  
print(resultado)
```











