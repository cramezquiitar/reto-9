# reto-9
### Desarrollo del Reto:
1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
```python  
  # Ingresar la cantidad de datos a promediar
cantidad_valores = int(input("Cantidad de valores a promediar: "))

# Crear una lista para guardar los valores reales ingresados
lista_valores = []

# Solicitar los valores al usuario uno por uno
for indice in range(cantidad_valores):
    valor_real = float(input("Ingrese el valor " + str(indice + 1) + ": "))
    lista_valores.append(valor_real)

# Inicializar la variable para la suma total
suma_total = 0

# Sumar todos los valores de la lista
for valor in lista_valores:
    suma_total += valor

# Verificar que la cantidad sea mayor a cero para evitar división por cero
if cantidad_valores > 0:
    promedio = suma_total / cantidad_valores
    print("El promedio es:", promedio)
else:
    print("No hay valores para calcular el promedio.")
```
2. Desarrollar un algoritmo que calcule el [producto punto](https://www.cuemath.com/algebra/dot-product/) de dos arreglos de números enteros (reales) de igual tamaño# Paso 1: Ingresar la cantidad de elementos en los arreglos
```python
# Paso 1: Ingresar la cantidad de elementos en los arreglos
cantidad_elementos = int(input("Ingrese la cantidad de elementos en los arreglos: "))

# Paso 2: Crear las listas para almacenar los dos arreglos
arreglo_1 = []
arreglo_2 = []

# Paso 3: Ingresar los elementos del primer arreglo
print("Ingrese los elementos del primer arreglo:")
for i in range(cantidad_elementos):
    numero = float(input("Ingrese el valor " + str(i + 1) + " del arreglo 1: "))
    arreglo_1.append(numero)

# Paso 4: Ingresar los elementos del segundo arreglo
print("Ingrese los elementos del segundo arreglo:")
for i in range(cantidad_elementos):
    numero = float(input("Ingrese el valor " + str(i + 1) + " del arreglo 2: "))
    arreglo_2.append(numero)

# Paso 5: Calcular el producto punto
producto_punto = 0
for i in range(cantidad_elementos):
    producto_punto += arreglo_1[i] * arreglo_2[i]

# Paso 6: Mostrar el resultado
print("El producto punto de los dos arreglos es: " + str(producto_punto))
```
3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
```python
# Ingresar el tamaño del arreglo
cantidad = int(input("Ingrese la cantidad de elementos del arreglo: "))

# Crear el arreglo
arreglo = []

# Llenar el arreglo con los valores ingresados por el usuario
for n in range(cantidad):
    numero = int(input("Ingresar el número " + str(n + 1) + ": "))
    arreglo.append(numero)

# Crear un nuevo arreglo para los números distintos de cero
no_ceros = []

# Contar cuántos ceros hay
contador_ceros = 0
for n in range(cantidad):
    if arreglo[n] != 0:
        no_ceros.append(arreglo[n])
    else:
        contador_ceros = contador_ceros + 1

# Agregar los ceros al final del nuevo arreglo
for n in range(contador_ceros):
    no_ceros.append(0)

# Mostrar el resultado final
print("El arreglo con los ceros al final es: " + str(no_ceros))
```
4. Revisar que son los algoritmos de *sorting*, entender *bubble-sort* ([enlace](https://www.geeksforgeeks.org/bubble-sort/) a implementación).
Los algoritmos de sorting (algoritmos de ordenamiento) son procedimientos o pasos lógicos diseñados para reorganizar los elementos de una estructura de datos (como una lista o un arreglo), con el fin de que queden en un orden específico, normalmente ascendente (de menor a mayor) o descendente (de mayor a menor).
