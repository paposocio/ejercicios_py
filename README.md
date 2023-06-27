**Problema 1: Población de dos países**
En 2022, el país A tiene una población de 25 millones de habitantes y el país B tiene una población de 18.9 millones. Las tasas de crecimiento anual de la población son del 2% y 3% respectivamente. Desarrolla un programa que imprima el año en que la población del país B superará a la del país A.

**Solución:**
```python
poblacion_A = 25
poblacion_B = 18.9
tasa_crecimiento_A = 0.02
tasa_crecimiento_B = 0.03
año = 2022

while poblacion_A >= poblacion_B:
    poblacion_A += poblacion_A * tasa_crecimiento_A
    poblacion_B += poblacion_B * tasa_crecimiento_B
    año += 1

print("El año en que la población del país B supera a la de A es:", año)
```

**Problema 2: Listado de números y sus cuadrados**
Imprime un listado con los números del 1 al 100, cada uno con su respectivo cuadrado (es decir, cada número elevado al cuadrado).

**Solución:**
```python
for numero in range(1, 101):
    cuadrado = numero ** 2
    print(numero, "al cuadrado es igual a", cuadrado)
```

**Problema 3: Determinar si una cadena es palíndromo**
Desarrolla un algoritmo que determine si una cadena de caracteres es palíndromo. Una cadena se dice palíndromo si al invertirla es igual a ella misma.

**Solución:**
```python
def es_palindromo(cadena):
    cadena = cadena.lower()  # Convertir la cadena a minúsculas
    cadena = cadena.replace(" ", "")  # Eliminar espacios en blanco
    cadena_invertida = cadena[::-1]  # Invertir la cadena
    
    if cadena == cadena_invertida:
        return True
    else:
        return False

cadena = input("Ingrese una cadena de caracteres: ")
if es_palindromo(cadena):
    print("La cadena es un palíndromo.")
else:
    print("La cadena no es un palíndromo.")
```

**Problema 4: Cálculo de potencia**
Leer un número natural n y leer otro dato de tipo real x. Calcular x^n.

**Solución:**
```python
n = int(input("Ingrese un número natural n: "))
x = float(input("Ingrese un número real x: "))

resultado = x ** n

print(f"El resultado de elevar {x} a la potencia {n} es: {resultado}")
```
