"""
Misión: "Monitoreo de Pulso"
Objetivo: Usar while.
Crea un programa que pida el pulso del paciente. Mientras el pulso sea menor a 60, debe imprimir "Advertencia: Pulso bajo. 
Incrementando dosis..." y sumar 5 al pulso actual hasta llegar a 60. Al final, imprimir "Pulso estabilizado".
"""
# Pedir el pulso inicial al usuario
pulso = int(input("Ingrese el pulso del paciente: "))

# Mientras el pulso sea menor a 60, aplicar tratamiento
while pulso < 60:
    print(f"Advertencia: Pulso bajo. Incrementando dosis... Pulso actual: {pulso}")
    pulso = pulso + 5

# Al salir del bucle, el pulso ya es >= 60
print(f"Pulso estabilizado en {pulso}")

"""
Misión "Impresión en Serie de Vigas"
Objetivo: Usar for y range().
Tu impresora 3D (como las de tu granja ImpreXpress) debe fabricar 10 vigas para un puente. 
Crea un programa que imprima: Fabricando viga #1... Fabricando viga #2... (Hasta llegar a la viga #10). 
Al terminar, debe decir "Estructura completada".
"""
# Usamos range(1, 11) para generar números del 1 al 10
# (El segundo número, 11, es el límite y no se incluye)
for i in range(1, 11):
    print(f"Fabricando viga #{i}...")

# Mensaje final fuera del bucle
print("Estructura completada")

"""
Misión "Conteo de Población"
Objetivo: Usar acumuladores/contadores.
El sistema debe recibir la edad de 5 ciudadanos uno por uno. 
Al final, el programa debe mostrar cuántos de esos 5 son mayores de edad (usando un if dentro del for).
"""
# Inicializamos el contador de mayores de edad en 0
contador_mayores = 0

# Usamos un bucle for para pedir la edad de 5 ciudadanos
for i in range(1, 6):
    edad = int(input(f"Ingrese la edad del ciudadano #{i}: "))
    
    # Verificamos si es mayor de edad (18 años o más)
    if edad >= 18:
        contador_mayores += 1  # Sumamos 1 al contador si la condición es verdadera

# Al terminar el bucle, mostramos el total acumulado
print(f"Total de mayores de edad: {contador_mayores}")
