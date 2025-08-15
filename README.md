¡Hola! voy a dejar aqui la practica de la unidad 1 a modo de texto para facil acceso o en caso de solo querer comparar algo mas puntual y el archivo correspondiente en su formato .py en caso de que quieran probarlo o modificarlo de forma directa. ¡Mucha suerte a todos! 

# 1) Crear un programa que imprima por pantalla el mensaje: "Hola Mundo!"

print("Hola Mundo!")

#=====================================================================================================================================

# 2)Crear un programa que solicite un nombre al usuario y le devuelva un saludo

usuario = input("Ingrese su nombre: ")
print(f"¡Hola {usuario}!")

#=====================================================================================================================================

# 3) Crear un programa que solicite: nombre, apellido, edad y residencia 
# y arme una oracion con los datos

a, b, c, d = input("Ingrese su nombre: "), input("Ingrese su apellido: "), input("Ingrese su edad: "), input("Ingrese donde vive: ")
print(f"Mi nombre es {a} {b}, tengo {str(c)} años y vivo en {d}")

#=====================================================================================================================================

# 4) Crear un programa que pida un radio de un circulo y devuelva su area y perimetro

radio = float(input("Ingrese el radio del circulo: "))
pi = 3.14

area = round(pi * (radio * radio), 2)
perimetro = round(pi * (2 * radio), 2)

print(f"El area del circulo es: {str(area)} y el perimetro es: {str(perimetro)}")

#=====================================================================================================================================

# 5) Crear un programa que pida segundos y los transforme en horas

segundos = float(input("Ingrese una cantidad de segundos: "))
horas = int(segundos / 3600)
print(f"Esos segundos equivalen a: {str(horas)} horas")

#=====================================================================================================================================

# 6) Crear un programa que pida al usuario un numero
# e imprima por pantalla la tabla de multiplicar del mismo

num = int(input("Ingrese un numero: "))

print(f"{str(num)} x 1 = {num * 1}")
print(f"{str(num)} x 2 = {num * 2}")
print(f"{str(num)} x 3 = {num * 3}")
print(f"{str(num)} x 4 = {num * 4}")
print(f"{str(num)} x 5 = {num * 5}")
print(f"{str(num)} x 6 = {num * 6}")
print(f"{str(num)} x 7 = {num * 7}")
print(f"{str(num)} x 8 = {num * 8}")
print(f"{str(num)} x 9 = {num * 9}")
print(f"{str(num)} x 10 = {num * 10}")

#Otra forma de hacerlo

num = int(input("Ingrese un numero: "))

for i in range(1, 11):
    resultado = num * i
    print(f"{num} x {i} = {resultado}")

#=====================================================================================================================================

# 7) crear un programa que pida 2 numeros enteros distintos de 0 y devuelva
# suma, resta, division y multiplicacion

a = float(input("Ingrese un numero entero: "))

if a < 1:
    
    while a < 1:
        print("Por favor ingrese un valor mayor a 0")
        a = float(input("Ingrese un numero entero: "))

b = float(input("Ingrese otro numero entero: "))

if b < 1:
    while b < 1:
        print("Por favor ingrese un valor mayor a 0")
        b = float(input("Ingrese otro numero entero: "))
    
suma = round(a + b, 2)
resta = round(a - b, 2)
division = round(a / b, 2)
multiplicacion = round(a * b, 2)

print(f"{str(a)} + {str(b)} = {str(suma)}")
print(f"{str(a)} - {str(b)} = {str(resta)}")
print(f"{str(a)} / {str(b)} = {str(division)}")
print(f"{str(a)} * {str(b)} = {str(multiplicacion)}")
    
#=====================================================================================================================================

# 8) Crear un programa para calcular el indice de masa corporal

peso = float(input("Ingrese su peso actual: "))
altura = float(input("Ingrese su altura actual: "))

imc = round(peso / altura ** 2, 2)

print(f"Su indice de masa corporal es de: {imc}")

#=====================================================================================================================================

# 9) Crear un programa que pase la temperatura de grados Celsius
# a grados Fahrenheit

cels = float(input("Ingrese la temperatura en Celsius: "))
fahr = round((9/5) * cels + 32, 2)

print(f"La temperatura en grados Fahrenheit es: {fahr}°F")

#=====================================================================================================================================

# 10) Crear un programa que devuelva el promedio de 3 numeros
# otorgados por el usuario

n1 = float(input("Ingrese su primera nota: "))

if n1 < 0:
    
    while n1 < 0:
        print("Por favor ingrese una nota valida")
        n1 = float(input("Ingrese su primera nota: "))
        
n2 = float(input("Ingrese el segundo numero: "))

if n2 < 0:
    
    while n2 < 0:
        print("Por favor ingrese una nota valida")
        n2 = float(input("Ingrese su primera nota: "))

n3 = float(input("Ingrese el tercer numero: "))

if n3 < 0:
    
    while n3 < 0:
        print("Por favor ingrese una nota valida")
        n3 = float(input("Ingrese su primera nota: "))

promedio = round((n1 + n2 + n3) / 3)

print(f"El promedio es: {promedio}")