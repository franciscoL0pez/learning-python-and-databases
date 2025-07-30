# Python desde Cero: Guía para Principiantes 🐍

## ¿Qué es Python?

Python es un lenguaje de programación de alto nivel, interpretado y de propósito general. Fue creado por Guido van Rossum en 1991 y se ha convertido en uno de los lenguajes más populares del mundo. 🌟

### ¿Por qué aprender Python?

- **Fácil de aprender**: Sintaxis simple y legible 📚
- **Versátil**: Usado en desarrollo web, ciencia de datos, inteligencia artificial, automatización, etc.
- **Gran comunidad**: Millones de desarrolladores y recursos disponibles 🤝
- **Muchas oportunidades laborales**: Alta demanda en el mercado 💼

## Instalación

### Windows
1. Ve a [python.org](https://python.org)
2. Descarga la última versión
3. Ejecuta el instalador y marca "Add Python to PATH"

### Mac/Linux
Python suele venir preinstalado. Verifica con:
```bash
python3 --version
```

## Conceptos Básicos 📖

### Variables: Los Contenedores de Información 📦

Las **variables** son como cajas etiquetadas donde guardas información. Imagina que tienes cajas en tu cuarto: una dice "libros", otra "ropa", otra "juguetes". Las variables funcionan igual: son contenedores con nombres que guardan diferentes tipos de información.

**¿Para qué sirven las variables?**
- Almacenar datos que puedes usar más tarde
- Hacer que tu código sea más legible y organizado
- Permitir que los datos cambien durante la ejecución del programa

```python
# Crear variables es como etiquetar cajas
nombre = "Juan"           # Una caja llamada "nombre" con el texto "Juan"
edad = 25                # Una caja llamada "edad" con el número 25
altura = 1.75            # Una caja llamada "altura" con el decimal 1.75
es_estudiante = True     # Una caja llamada "es_estudiante" con verdadero/falso

# Puedes cambiar el contenido de las cajas
edad = 26               # Ahora la caja "edad" contiene 26 en lugar de 25
print(f"Mi nombre es {nombre} y tengo {edad} años")
```

**Reglas para nombrar variables:**
```python
# ✅ Correcto
mi_nombre = "Ana"
edad_usuario = 30
numero_1 = 10

# ❌ Incorrecto
2numero = 10      # No puede empezar con número
mi-nombre = "Ana" # No puede tener guiones
class = "Python"  # No puede usar palabras reservadas
```

### Tipos de Datos: Los Diferentes Tipos de Información 🗃️

Python maneja diferentes tipos de información, como diferentes tipos de objetos en la vida real:

#### 1. Números (int y float)
```python
# Enteros (int) - números sin decimales
edad = 25
cantidad_hermanos = 3
temperatura = -5

# Decimales (float) - números con punto decimal
altura = 1.75
precio = 19.99
pi = 3.14159

# ¿Para qué sirven?
# - Hacer cálculos matemáticos
# - Contar elementos
# - Medir cantidades
print(f"Si tienes {edad} años, el próximo año tendrás {edad + 1}")
```

#### 2. Texto (string o str)
```python
# Los strings guardan texto, siempre entre comillas
nombre = "María"
apellido = 'García'           # Comillas simples también funcionan
mensaje = "Hola, ¿cómo estás?"
direccion = "Calle Falsa 123"

# ¿Para qué sirven?
# - Almacenar nombres, mensajes, direcciones
# - Mostrar información al usuario
# - Procesar y manipular texto

# Puedes combinar (concatenar) strings
nombre_completo = nombre + " " + apellido
print(f"Nombre completo: {nombre_completo}")   # María García

# También puedes hacer esto (más moderno):
presentacion = f"Hola, soy {nombre} y vivo en {direccion}"
```

#### 3. Booleanos (bool) - Verdadero o Falso
```python
# Solo pueden ser True (verdadero) o False (falso)
es_estudiante = True
tiene_mascota = False
mayor_de_edad = True

# ¿Para qué sirven?
# - Tomar decisiones en el programa
# - Representar estados (encendido/apagado, sí/no)
# - Controlar el flujo del programa

if es_estudiante:
    print("Tienes descuento estudiantil")
else:
    print("Precio regular")
```

#### 4. Listas - Colecciones Ordenadas 📋
```python
# Las listas guardan múltiples elementos en orden
frutas = ["manzana", "banana", "naranja", "uva"]
numeros = [1, 2, 3, 4, 5]
mixta = ["Juan", 25, True, 1.75]  # Puede mezclar tipos

# ¿Para qué sirven?
# - Guardar múltiples elementos relacionados
# - Mantener un orden específico
# - Procesar grupos de datos

print(f"Tengo {len(frutas)} frutas")        # Cuenta elementos
print(f"Mi fruta favorita es {frutas[0]}")  # Accede al primer elemento
frutas.append("pera")                       # Agrega un elemento
print(f"Ahora tengo: {frutas}")
```

#### 5. Diccionarios - Pares Clave-Valor 🗂️
```python
# Los diccionarios guardan información relacionada en pares clave:valor
persona = {
    "nombre": "Ana",
    "edad": 30,
    "ciudad": "Madrid",
    "es_estudiante": False
}

# ¿Para qué sirven?
# - Organizar información relacionada
# - Acceder rápidamente a datos específicos
# - Representar objetos del mundo real

print(f"Nombre: {persona['nombre']}")        # Accede por clave
print(f"Edad: {persona['edad']} años")
persona["edad"] = 31                         # Modifica un valor
persona["telefono"] = "123-456-789"          # Agrega nueva información
```

### Operaciones Básicas: Manipulando los Datos 🔧

Las operaciones te permiten trabajar con los datos, transformarlos y combinarlos:

```python
# Operaciones matemáticas
suma = 5 + 3           # 8 - Suma dos números
resta = 10 - 4         # 6 - Resta el segundo del primero
multiplicacion = 3 * 7  # 21 - Multiplica dos números
division = 15 / 3      # 5.0 - Divide (siempre da decimal)
division_entera = 15 // 3  # 5 - División que da número entero
modulo = 17 % 5        # 2 - El "resto" de la división (17 ÷ 5 = 3, resto 2)
potencia = 2 ** 3      # 8 - Dos elevado a la tercera potencia

# Trabajando con texto
saludo = "Hola " + "mundo"     # "Hola mundo" - Une textos
repetir = "Ja" * 3             # "JaJaJa" - Repite texto
texto_largo = "Python es genial"
mayusculas = texto_largo.upper()     # "PYTHON ES GENIAL"
minusculas = texto_largo.lower()     # "python es genial"
longitud = len(texto_largo)          # 16 - Cuenta caracteres

# Trabajando con listas
frutas = ["manzana", "banana", "naranja"]
cantidad_frutas = len(frutas)        # 3 - Cuenta elementos
primera_fruta = frutas[0]            # "manzana" - Primer elemento
ultima_fruta = frutas[-1]            # "naranja" - Último elemento
```

**Ejemplo práctico: Calculadora de propina**
```python
precio_comida = 50.0
porcentaje_propina = 15
propina = precio_comida * (porcentaje_propina / 100)
total = precio_comida + propina
print(f"Comida: ${precio_comida}")
print(f"Propina ({porcentaje_propina}%): ${propina}")
print(f"Total: ${total}")
```

## Estructuras de Control: Tomando Decisiones y Repitiendo Acciones 🔄

Las estructuras de control son como los semáforos y las señales de tráfico en tu código: deciden qué camino tomar y cuándo repetir acciones.

### Condicionales (if/else): Tomando Decisiones 🚦

Los condicionales permiten que tu programa tome decisiones basadas en diferentes situaciones:

#### Condicional Básico
```python
edad = 18

if edad >= 18:
    print("Eres mayor de edad")
    print("Puedes votar")
else:
    print("Eres menor de edad")
    print("Aún no puedes votar")

# ¿Para qué sirven?
# - Ejecutar código solo si se cumple una condición
# - Hacer que el programa responda diferente según la situación
# - Validar datos antes de procesarlos
```

#### Múltiples Condiciones (elif)
```python
calificacion = 85

if calificacion >= 90:
    print("¡Excelente! 🌟")
    descuento = 20  # Descuento en próxima matrícula
elif calificacion >= 80:
    print("Muy bien 👍")
    descuento = 10
elif calificacion >= 70:
    print("Bien ✓")
    descuento = 5
elif calificacion >= 60:
    print("Suficiente")
    descuento = 0
else:
    print("Necesitas estudiar más 📚")
    descuento = 0

print(f"Tu descuento es: {descuento}%")
```

#### Condiciones Complejas
```python
temperatura = 25
llueve = False
fin_de_semana = True

# Usando operadores lógicos: and, or, not
if temperatura > 20 and not llueve:
    print("Perfecto para salir")
    if fin_de_semana:
        print("¡Y es fin de semana! 🎉")
elif temperatura > 15 or fin_de_semana:
    print("Puede ser un buen día para salir")
else:
    print("Mejor quedarse en casa")
```

### Bucles: Repitiendo Acciones 🔁

Los bucles permiten repetir código múltiples veces sin escribirlo una y otra vez:

#### Bucle For: Repetir un Número Específico de Veces
```python
# Repetir 5 veces
print("Contando del 0 al 4:")
for i in range(5):
    print(f"Número: {i}")

# Personalizar el rango
print("\nContando del 1 al 10:")
for numero in range(1, 11):  # Desde 1 hasta 10 (11 no incluido)
    print(f"Número: {numero}")

# Contar de 2 en 2
print("\nNúmeros pares del 0 al 10:")
for par in range(0, 11, 2):  # Desde 0 hasta 10, saltando de 2 en 2
    print(par)
```

#### Recorrer Listas y Strings
```python
# Recorrer una lista
frutas = ["manzana", "banana", "naranja", "uva"]
print("Mis frutas favoritas:")
for fruta in frutas:
    print(f"- Me gusta la {fruta}")

# Recorrer con índice (posición)
print("\nFrutas numeradas:")
for indice, fruta in enumerate(frutas):
    print(f"{indice + 1}. {fruta}")

# Recorrer un string (letra por letra)
palabra = "Python"
print(f"\nLetras en '{palabra}':")
for letra in palabra:
    print(f"- {letra}")
```

#### Bucle While: Repetir Mientras se Cumpla una Condición
```python
# Contar hasta que llegue a un límite
contador = 0
limite = 3

print("Contando con while:")
while contador < limite:
    print(f"Contador: {contador}")
    contador += 1  # MUY IMPORTANTE: aumentar el contador para evitar bucle infinito

# Ejemplo práctico: Pedir datos hasta que sean válidos
password_correcta = "secreto123"
intentos = 0
max_intentos = 3

while intentos < max_intentos:
    password = input("Ingresa la contraseña: ")
    if password == password_correcta:
        print("¡Acceso concedido! ✅")
        break  # Sale del bucle
    else:
        intentos += 1
        restantes = max_intentos - intentos
        if restantes > 0:
            print(f"Contraseña incorrecta. Te quedan {restantes} intentos")
        else:
            print("Se agotaron los intentos. Acceso denegado ❌")
```

#### Bucles Anidados (Bucles dentro de Bucles)
```python
# Tabla de multiplicar
print("Tabla de multiplicar del 1 al 3:")
for numero in range(1, 4):  # Del 1 al 3
    print(f"\nTabla del {numero}:")
    for multiplicador in range(1, 6):  # Del 1 al 5
        resultado = numero * multiplicador
        print(f"{numero} x {multiplicador} = {resultado}")
```

#### Control de Flujo en Bucles
```python
# break: Sale completamente del bucle
# continue: Salta a la siguiente iteración

numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

print("Números menores a 6:")
for numero in numeros:
    if numero == 6:
        break  # Sale del bucle cuando encuentra 6
    print(numero)

print("\nSolo números impares:")
for numero in numeros:
    if numero % 2 == 0:  # Si es par
        continue  # Salta esta iteración
    print(numero)  # Solo imprime los impares
```

## Funciones: Bloques de Código Reutilizable 🔧

Las **funciones** son como pequeñas máquinas que toman información (entrada), hacen algo con ella, y pueden devolver un resultado (salida). Imagina una función como una licuadora: le das frutas (entrada), las procesa, y te devuelve un batido (salida).

### ¿Para qué sirven las funciones?

1. **Evitar repetir código**: En lugar de escribir el mismo código varias veces
2. **Organizar el programa**: Dividir problemas grandes en partes pequeñas
3. **Reutilizar código**: Usar la misma función en diferentes partes del programa
4. **Facilitar el mantenimiento**: Si necesitas cambiar algo, solo lo cambias en un lugar

### Anatomía de una Función

```python
def nombre_de_la_funcion(parametros):
    """Documentación opcional: qué hace la función"""
    # Código que hace el trabajo
    return resultado  # Opcional: devuelve algo
```

### Funciones Básicas

#### 1. Función Simple (sin parámetros, sin retorno)
```python
def saludar():
    """Esta función simplemente muestra un saludo"""
    print("¡Hola! Bienvenido al programa")
    print("Espero que tengas un buen día")

# Para usar la función, la "llamamos"
saludar()  # Esto ejecuta todo el código dentro de la función
```

#### 2. Función con Parámetros (recibe información)
```python
def saludar_persona(nombre):
    """Esta función saluda a una persona específica"""
    print(f"¡Hola, {nombre}!")
    print("Es un placer conocerte")

# Llamamos la función pasándole un nombre
saludar_persona("María")    # ¡Hola, María!
saludar_persona("Carlos")   # ¡Hola, Carlos!

# Múltiples parámetros
def presentar_persona(nombre, edad, ciudad):
    """Presenta a una persona con sus datos"""
    print(f"Te presento a {nombre}")
    print(f"Tiene {edad} años y vive en {ciudad}")

presentar_persona("Ana", 25, "Barcelona")
```

#### 3. Función que Devuelve un Valor (return)
```python
def sumar(a, b):
    """Suma dos números y devuelve el resultado"""
    resultado = a + b
    return resultado  # Devuelve el valor para usarlo después

# Guardamos el resultado en una variable
total = sumar(5, 3)      # total vale 8
print(f"La suma es: {total}")

# O lo usamos directamente
print(f"5 + 7 = {sumar(5, 7)}")  # 5 + 7 = 12
```

#### 4. Funciones Más Complejas
```python
def calculadora(numero1, numero2, operacion):
    """
    Calculadora simple que puede sumar, restar, multiplicar o dividir
    
    Parámetros:
    - numero1: primer número
    - numero2: segundo número  
    - operacion: "suma", "resta", "multiplicacion", "division"
    
    Devuelve:
    - El resultado de la operación
    """
    if operacion == "suma":
        return numero1 + numero2
    elif operacion == "resta":
        return numero1 - numero2
    elif operacion == "multiplicacion":
        return numero1 * numero2
    elif operacion == "division":
        if numero2 != 0:  # Evitar división por cero
            return numero1 / numero2
        else:
            return "Error: No se puede dividir por cero"
    else:
        return "Operación no válida"

# Ejemplos de uso
print(calculadora(10, 5, "suma"))          # 15
print(calculadora(10, 5, "division"))      # 2.0
print(calculadora(10, 0, "division"))      # Error: No se puede dividir por cero
```

#### 5. Funciones con Valores por Defecto
```python
def crear_usuario(nombre, edad, ciudad="No especificada"):
    """
    Crea un perfil de usuario
    Si no se especifica ciudad, usa "No especificada"
    """
    perfil = f"Usuario: {nombre}, {edad} años, vive en {ciudad}"
    return perfil

# Puedes llamarla con o sin el último parámetro
usuario1 = crear_usuario("Juan", 30, "Madrid")        # Con ciudad
usuario2 = crear_usuario("María", 25)                 # Sin ciudad
print(usuario1)  # Usuario: Juan, 30 años, vive en Madrid
print(usuario2)  # Usuario: María, 25 años, vive en No especificada
```

### Ejemplos Prácticos de Funciones

#### Función para Validar Email
```python
def es_email_valido(email):
    """Verifica si un email tiene formato básico válido"""
    if "@" in email and "." in email:
        return True
    else:
        return False

# Uso
email_usuario = "juan@gmail.com"
if es_email_valido(email_usuario):
    print("Email válido")
else:
    print("Email inválido")
```

#### Función para Calcular Descuentos
```python
def calcular_precio_final(precio_original, descuento_porcentaje=0):
    """
    Calcula el precio final después de aplicar descuento
    
    Parámetros:
    - precio_original: precio antes del descuento
    - descuento_porcentaje: porcentaje de descuento (0-100)
    
    Devuelve:
    - precio final después del descuento
    """
    descuento_monto = precio_original * (descuento_porcentaje / 100)
    precio_final = precio_original - descuento_monto
    return precio_final

# Ejemplos
precio_camisa = 50
precio_con_descuento = calcular_precio_final(precio_camisa, 20)  # 20% descuento
print(f"Precio original: ${precio_camisa}")
print(f"Precio con descuento: ${precio_con_descuento}")  # $40.0
```

#### Función que Procesa Listas
```python
def analizar_numeros(lista_numeros):
    """
    Analiza una lista de números y devuelve estadísticas
    
    Devuelve un diccionario con:
    - cantidad: cuántos números hay
    - suma: suma de todos los números
    - promedio: promedio de los números
    - mayor: número más grande
    - menor: número más pequeño
    """
    if not lista_numeros:  # Si la lista está vacía
        return "Lista vacía"
    
    estadisticas = {
        "cantidad": len(lista_numeros),
        "suma": sum(lista_numeros),
        "promedio": sum(lista_numeros) / len(lista_numeros),
        "mayor": max(lista_numeros),
        "menor": min(lista_numeros)
    }
    
    return estadisticas

# Uso
notas = [85, 90, 78, 92, 88]
resultado = analizar_numeros(notas)
print(f"Estadísticas de las notas:")
for clave, valor in resultado.items():
    print(f"{clave}: {valor}")
```

### ¿Por qué son Importantes las Funciones? 🤔

```python
# SIN funciones (código repetitivo y desorganizado)
precio1 = 100
descuento1 = precio1 * 0.15
precio_final1 = precio1 - descuento1
print(f"Producto 1: ${precio_final1}")

precio2 = 75
descuento2 = precio2 * 0.15
precio_final2 = precio2 - descuento2
print(f"Producto 2: ${precio_final2}")

precio3 = 200
descuento3 = precio3 * 0.15
precio_final3 = precio3 - descuento3
print(f"Producto 3: ${precio_final3}")

# CON funciones (código limpio y reutilizable)
def aplicar_descuento(precio, porcentaje=15):
    descuento = precio * (porcentaje / 100)
    return precio - descuento

# Mucho más simple y limpio
productos = [100, 75, 200]
for i, precio in enumerate(productos, 1):
    precio_final = aplicar_descuento(precio)
    print(f"Producto {i}: ${precio_final}")
```

## Trabajando con Listas: Tu Colección de Datos 📋

Las listas son una de las estructuras de datos más importantes en Python. Son como contenedores ordenados donde puedes guardar múltiples elementos.

### ¿Qué son las Listas y Para Qué Sirven?

Las listas son colecciones **ordenadas** y **mutables** (se pueden cambiar) de elementos. Imagínalas como:
- Una lista de compras
- Una lista de contactos en tu teléfono
- Una playlist de música
- Un inventario de productos

### Creando y Manipulando Listas

#### Creación de Listas
```python
# Lista vacía
lista_vacia = []
otra_lista_vacia = list()

# Lista con elementos
numeros = [1, 2, 3, 4, 5]
frutas = ["manzana", "banana", "naranja", "uva"]
mixta = ["Juan", 25, True, 3.14]  # Puede contener diferentes tipos
colores = ["rojo", "verde", "azul", "amarillo", "morado"]

print(f"Tengo {len(frutas)} frutas en mi lista")  # len() cuenta elementos
```

#### Accediendo a Elementos (Indexación)
```python
frutas = ["manzana", "banana", "naranja", "uva"]

# Los índices empiezan en 0
primera_fruta = frutas[0]     # "manzana"
segunda_fruta = frutas[1]     # "banana"
ultima_fruta = frutas[-1]     # "uva" (índice negativo cuenta desde el final)
penultima = frutas[-2]        # "naranja"

print(f"Mi fruta favorita es la {primera_fruta}")
print(f"La última fruta es {ultima_fruta}")

# Verificar si un elemento existe
if "banana" in frutas:
    print("¡Sí tenemos bananas! 🍌")
```

#### Rebanadas (Slicing) - Obtener Partes de la Lista
```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

# lista[inicio:fin]  (fin no incluido)
primeros_tres = numeros[0:3]      # [0, 1, 2]
desde_medio = numeros[5:]         # [5, 6, 7, 8, 9]
hasta_medio = numeros[:5]         # [0, 1, 2, 3, 4]
ultimos_tres = numeros[-3:]       # [7, 8, 9]

# Con saltos: lista[inicio:fin:salto]
numeros_pares = numeros[::2]      # [0, 2, 4, 6, 8] (de 2 en 2)
reversa = numeros[::-1]           # [9, 8, 7, 6, 5, 4, 3, 2, 1, 0]

print(f"Primeros tres: {primeros_tres}")
print(f"Lista al revés: {reversa}")
```

#### Modificando Listas

```python
frutas = ["manzana", "banana", "naranja"]

# Agregar elementos
frutas.append("uva")              # Agrega al final: ["manzana", "banana", "naranja", "uva"]
frutas.insert(1, "pera")          # Inserta en posición 1: ["manzana", "pera", "banana", "naranja", "uva"]

# Agregar múltiples elementos
mas_frutas = ["kiwi", "mango"]
frutas.extend(mas_frutas)         # ["manzana", "pera", "banana", "naranja", "uva", "kiwi", "mango"]

# Modificar elementos existentes
frutas[0] = "manzana verde"       # Cambia el primer elemento

# Eliminar elementos
frutas.remove("banana")           # Elimina la primera ocurrencia de "banana"
fruta_eliminada = frutas.pop()    # Elimina y devuelve el último elemento
fruta_especifica = frutas.pop(1)  # Elimina y devuelve el elemento en posición 1

print(f"Lista actual: {frutas}")
print(f"Eliminé: {fruta_eliminada}")
```

#### Métodos Útiles de Listas

```python
numeros = [3, 1, 4, 1, 5, 9, 2, 6]

# Información sobre la lista
cantidad = len(numeros)           # 8 - número de elementos
suma_total = sum(numeros)         # 31 - suma de todos los elementos
mayor = max(numeros)              # 9 - elemento más grande
menor = min(numeros)              # 1 - elemento más pequeño
cuenta_1 = numeros.count(1)       # 2 - cuántas veces aparece el 1

# Ordenar
numeros_ordenados = sorted(numeros)    # Nueva lista ordenada: [1, 1, 2, 3, 4, 5, 6, 9]
numeros.sort()                         # Ordena la lista original
numeros.reverse()                      # Invierte el orden

print(f"Números ordenados: {numeros_ordenados}")
print(f"Estadísticas: suma={suma_total}, promedio={suma_total/cantidad}")
```

#### Listas de Comprensión (List Comprehensions) - Técnica Avanzada
```python
# Forma tradicional de crear una lista de cuadrados
cuadrados = []
for numero in range(1, 6):
    cuadrados.append(numero ** 2)
print(cuadrados)  # [1, 4, 9, 16, 25]

# Forma más elegante con list comprehension
cuadrados = [numero ** 2 for numero in range(1, 6)]
print(cuadrados)  # [1, 4, 9, 16, 25]

# Con condiciones
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
pares = [num for num in numeros if num % 2 == 0]
print(f"Números pares: {pares}")  # [2, 4, 6, 8, 10]

# Procesando strings
nombres = ["juan", "maría", "carlos", "ana"]
nombres_capitalizados = [nombre.capitalize() for nombre in nombres]
print(nombres_capitalizados)  # ['Juan', 'María', 'Carlos', 'Ana']
```

### Ejemplos Prácticos con Listas

#### Sistema de Inventario Simple
```python
def gestionar_inventario():
    """Sistema simple de gestión de inventario"""
    inventario = []
    
    while True:
        print("\n--- INVENTARIO ---")
        print("1. Agregar producto")
        print("2. Ver inventario")
        print("3. Buscar producto")
        print("4. Eliminar producto")
        print("5. Salir")
        
        opcion = input("Selecciona una opción: ")
        
        if opcion == "1":
            producto = input("Nombre del producto: ")
            inventario.append(producto)
            print(f"✅ {producto} agregado al inventario")
            
        elif opcion == "2":
            if inventario:
                print(f"\n📦 Tienes {len(inventario)} productos:")
                for i, producto in enumerate(inventario, 1):
                    print(f"{i}. {producto}")
            else:
                print("📭 Inventario vacío")
                
        elif opcion == "3":
            buscar = input("¿Qué producto buscas? ")
            if buscar in inventario:
                posicion = inventario.index(buscar) + 1
                print(f"✅ {buscar} encontrado en posición {posicion}")
            else:
                print(f"❌ {buscar} no está en el inventario")
                
        elif opcion == "4":
            if inventario:
                print("Productos disponibles:")
                for i, producto in enumerate(inventario, 1):
                    print(f"{i}. {producto}")
                try:
                    indice = int(input("Número del producto a eliminar: ")) - 1
                    producto_eliminado = inventario.pop(indice)
                    print(f"🗑️ {producto_eliminado} eliminado")
                except (ValueError, IndexError):
                    print("❌ Número inválido")
            else:
                print("📭 No hay productos para eliminar")
                
        elif opcion == "5":
            print("👋 ¡Hasta luego!")
            break
        else:
            print("❌ Opción inválida")

# Para usar la función:
# gestionar_inventario()
```

#### Analizador de Calificaciones
```python
def analizar_calificaciones(calificaciones):
    """Analiza una lista de calificaciones y proporciona estadísticas"""
    if not calificaciones:
        return "No hay calificaciones para analizar"
    
    # Estadísticas básicas
    total_estudiantes = len(calificaciones)
    suma = sum(calificaciones)
    promedio = suma / total_estudiantes
    mas_alta = max(calificaciones)
    mas_baja = min(calificaciones)
    
    # Contar por rangos
    excelentes = [cal for cal in calificaciones if cal >= 90]
    buenas = [cal for cal in calificaciones if 80 <= cal < 90]
    regulares = [cal for cal in calificaciones if 70 <= cal < 80]
    bajas = [cal for cal in calificaciones if cal < 70]
    
    # Crear reporte
    reporte = f"""
📊 REPORTE DE CALIFICACIONES
{'='*30}
👥 Total de estudiantes: {total_estudiantes}
📈 Promedio de la clase: {promedio:.1f}
🏆 Calificación más alta: {mas_alta}
📉 Calificación más baja: {mas_baja}

📋 DISTRIBUCIÓN:
🌟 Excelentes (90+): {len(excelentes)} estudiantes
👍 Buenas (80-89): {len(buenas)} estudiantes  
✓ Regulares (70-79): {len(regulares)} estudiantes
📚 Necesitan apoyo (<70): {len(bajas)} estudiantes
    """
    
    return reporte

# Ejemplo de uso
notas_clase = [85, 92, 78, 96, 87, 73, 89, 94, 81, 76, 88, 91]
print(analizar_calificaciones(notas_clase))
```

## Entrada y Salida: Comunicándote con el Usuario 💬

La entrada y salida permiten que tu programa interactúe con las personas. Es como tener una conversación:

### Mostrar Información (Salida)
```python
# print() es tu herramienta principal para mostrar información
print("Hola mundo")
print("Mi nombre es Python")

# Mostrar variables
nombre = "María"
edad = 25
print("Mi nombre es", nombre)
print("Tengo", edad, "años")

# Formato moderno con f-strings (más legible)
print(f"Hola, soy {nombre} y tengo {edad} años")

# Personalizar el output
print("Uno", "Dos", "Tres", sep=" - ")  # Uno - Dos - Tres
print("Esta línea no termina en salto", end="... ")
print("y continúa aquí")
```

### Recibir Información (Entrada)
```python
# input() siempre devuelve texto (string)
nombre = input("¿Cuál es tu nombre? ")
print(f"¡Hola, {nombre}! 👋")

# Convertir a números
edad_texto = input("¿Cuántos años tienes? ")
edad = int(edad_texto)  # Convierte texto a número entero
print(f"El próximo año tendrás {edad + 1} años")

# Forma más directa
altura = float(input("¿Cuál es tu altura en metros? "))  # Para decimales
print(f"Tu altura es {altura} metros")

# Validar entrada
while True:
    try:
        numero = int(input("Ingresa un número: "))
        break  # Sale del bucle si la conversión fue exitosa
    except ValueError:
        print("❌ Eso no es un número válido. Intenta de nuevo.")

print(f"Perfecto, ingresaste: {numero}")
```

## Ejercicios Prácticos 🎯

### Ejercicio 1: Calculadora Simple 🧮
```python
# Pide dos números al usuario y muestra la suma
numero1 = float(input("Ingresa el primer número: "))
numero2 = float(input("Ingresa el segundo número: "))
suma = numero1 + numero2
print(f"La suma es: {suma}")
```

### Ejercicio 2: Lista de Tareas 📝
```python
# Crear una lista de tareas simple
tareas = []

while True:
    accion = input("¿Qué quieres hacer? (agregar/mostrar/salir): ").lower()
    
    if accion == "agregar":
        tarea = input("Escribe la tarea: ")
        tareas.append(tarea)
        print("Tarea agregada! ✅")
    
    elif accion == "mostrar":
        print("\nTus tareas:")
        for i, tarea in enumerate(tareas, 1):
            print(f"{i}. {tarea}")
    
    elif accion == "salir":
        print("¡Hasta luego! 👋")
        break
    
    else:
        print("Opción no válida ❌")
```

### Ejercicio 3: Juego de Adivinanza 🎲
```python
import random

numero_secreto = random.randint(1, 100)
intentos = 0

print("¡Adivina el número entre 1 y 100! 🤔")

while True:
    intento = int(input("Tu adivinanza: "))
    intentos += 1
    
    if intento == numero_secreto:
        print(f"¡Correcto! 🎉 Lo adivinaste en {intentos} intentos")
        break
    elif intento < numero_secreto:
        print("Muy bajo, intenta con un número mayor ⬆️")
    else:
        print("Muy alto, intenta con un número menor ⬇️")
```

## Manejo de Errores ⚠️

```python
# Usar try/except para manejar errores
try:
    numero = int(input("Ingresa un número: "))
    resultado = 10 / numero
    print(f"Resultado: {resultado}")
except ValueError:
    print("Error: Debes ingresar un número válido ❌")
except ZeroDivisionError:
    print("Error: No se puede dividir por cero ❌")
```

## Próximos Pasos 🚀

Una vez que domines estos conceptos básicos, puedes explorar:

### Conceptos Intermedios 📚
- **Programación orientada a objetos** (clases y objetos) - Organizar código como objetos del mundo real
- **Módulos y paquetes** - Reutilizar código y usar librerías
- **Manejo de archivos** - Leer y escribir archivos de texto, Excel, etc.
- **Comprensiones de listas** - Crear listas de forma más elegante y eficiente

### Librerías Populares 🛠️
- **NumPy**: Computación numérica y arrays
- **Pandas**: Análisis de datos y manipulación de tablas
- **Matplotlib**: Visualización de datos y gráficos
- **Django/Flask**: Desarrollo web y APIs
- **Requests**: Peticiones HTTP y consumo de APIs
- **Beautiful Soup**: Web scraping (extraer datos de páginas web)

### Recursos Recomendados 📖

**Documentación y Tutoriales:**
- [Documentación oficial de Python](https://docs.python.org/es/3/tutorial/) 📘
- [Python.org para principiantes](https://www.python.org/about/gettingstarted/) 🌟

**Plataformas de Práctica:**
- [HackerRank](https://www.hackerrank.com/domains/python) 💻
- [LeetCode](https://leetcode.com/) 🧩
- [Codewars](https://www.codewars.com/) ⚔️

**Cursos Online:**
- [Codecademy Python Course](https://www.codecademy.com/learn/learn-python-3) 🎓
- [freeCodeCamp](https://www.freecodecamp.org/) 🆓

## Consejos para Aprender 💡

1. **Practica diariamente**: Aunque sea 15-30 minutos ⏰
2. **Construye proyectos**: Aplica lo que aprendes en proyectos reales 🏗️
3. **Lee código de otros**: Estudia código en GitHub 👀
4. **Únete a comunidades**: Reddit r/Python, Stack Overflow 🤝
5. **No tengas miedo de los errores**: Son parte del aprendizaje 🚫😨
6. **Enseña lo que aprendes**: Explicar a otros solidifica tu conocimiento 🎯

## Conclusión 🎯

Python es un excelente primer lenguaje de programación. Su sintaxis clara y su versatilidad lo hacen ideal para principiantes. Recuerda que aprender a programar es como aprender un nuevo idioma: requiere práctica constante y paciencia.

¡Comienza con los ejercicios básicos y ve construyendo proyectos cada vez más complejos. El camino de mil millas comienza con un solo paso! 🌟

---

**¿Encontraste útil esta guía?** Contribuye al proyecto o compártela con otros principiantes. ¡La programación es más divertida cuando se aprende en comunidad! 🎉
