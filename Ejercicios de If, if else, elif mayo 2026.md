# Batería de 60 Ejemplos de Estructuras Condicionales en Python

**Nivel:** Preparatoria
**Entorno:** Visual Studio Code (VS Code)
**Tema:** Uso de `if`, `if else` y `elif`

---

# 1. Verificar si un número es positivo

```python
numero = 8

if numero > 0:
    print("El número es positivo")
```

---

# 2. Verificar mayoría de edad

```python
edad = 18

if edad >= 18:
    print("Eres mayor de edad")
```

---

# 3. Verificar si aprobó

```python
calificacion = 75

if calificacion >= 70:
    print("Aprobado")
```

---

# 4. Detectar temperatura alta

```python
temperatura = 32

if temperatura > 30:
    print("Hace mucho calor")
```

---

# 5. Comprobar contraseña correcta

```python
password = "1234"

if password == "1234":
    print("Acceso permitido")
```

---

# 6. Número par

```python
numero = 10

if numero % 2 == 0:
    print("Número par")
```

---

# 7. Número impar

```python
numero = 7

if numero % 2 != 0:
    print("Número impar")
```

---

# 8. Saldo suficiente

```python
saldo = 500

if saldo >= 300:
    print("Compra autorizada")
```

---

# 9. Alumno con asistencia completa

```python
asistencia = 100

if asistencia == 100:
    print("Reconocimiento por asistencia")
```

---

# 10. Velocidad excedida

```python
velocidad = 90

if velocidad > 80:
    print("Reduzca la velocidad")
```

---

# 11. Número positivo o negativo

```python
numero = -4

if numero >= 0:
    print("Positivo")
else:
    print("Negativo")
```

---

# 12. Aprobar o reprobar

```python
calificacion = 65

if calificacion >= 70:
    print("Aprobado")
else:
    print("Reprobado")
```

---

# 13. Entrar al cine

```python
edad = 15

if edad >= 13:
    print("Puede entrar")
else:
    print("No puede entrar")
```

---

# 14. Saldo bancario

```python
saldo = 200

if saldo >= 500:
    print("Retiro permitido")
else:
    print("Fondos insuficientes")
```

---

# 15. Número par o impar

```python
numero = 9

if numero % 2 == 0:
    print("Par")
else:
    print("Impar")
```

---

# 16. Clima

```python
llueve = True

if llueve:
    print("Lleva paraguas")
else:
    print("Disfruta el día")
```

---

# 17. Descuento en tienda

```python
compra = 1200

if compra >= 1000:
    print("Obtienes descuento")
else:
    print("Sin descuento")
```

---

# 18. Encender ventilador

```python
temperatura = 28

if temperatura > 25:
    print("Ventilador encendido")
else:
    print("Ventilador apagado")
```

---

# 19. Verificar usuario

```python
usuario = "admin"

if usuario == "admin":
    print("Bienvenido administrador")
else:
    print("Usuario normal")
```

---

# 20. Acceso a videojuego

```python
edad = 12

if edad >= 16:
    print("Acceso permitido")
else:
    print("Acceso restringido")
```

---

# 21. Clasificación de nota

```python
nota = 95

if nota >= 90:
    print("Excelente")
elif nota >= 80:
    print("Muy bien")
else:
    print("Necesita mejorar")
```

---

# 22. Semáforo

```python
color = "amarillo"

if color == "verde":
    print("Avanzar")
elif color == "amarillo":
    print("Precaución")
else:
    print("Detenerse")
```

---

# 23. Estación del año

```python
mes = 7

if mes in [12,1,2]:
    print("Invierno")
elif mes in [3,4,5]:
    print("Primavera")
else:
    print("Otra estación")
```

---

# 24. Nivel de batería

```python
bateria = 15

if bateria > 80:
    print("Carga alta")
elif bateria > 30:
    print("Carga media")
else:
    print("Carga baja")
```

---

# 25. Categoría por edad

```python
edad = 10

if edad < 13:
    print("Niño")
elif edad < 18:
    print("Adolescente")
else:
    print("Adulto")
```

---

# 26. Tipo de triángulo

```python
lado1 = 5
lado2 = 5
lado3 = 5

if lado1 == lado2 == lado3:
    print("Equilátero")
elif lado1 == lado2 or lado1 == lado3 or lado2 == lado3:
    print("Isósceles")
else:
    print("Escaleno")
```

---

# 27. Día laboral

```python
dia = "sábado"

if dia == "sábado":
    print("Fin de semana")
elif dia == "domingo":
    print("Fin de semana")
else:
    print("Día laboral")
```

---

# 28. Calificación con letras

```python
calificacion = 88

if calificacion >= 90:
    print("A")
elif calificacion >= 80:
    print("B")
else:
    print("C")
```

---

# 29. Temperatura ambiental

```python
temp = 18

if temp < 10:
    print("Frío")
elif temp < 25:
    print("Templado")
else:
    print("Caluroso")
```

---

# 30. Resultado deportivo

```python
goles = 3

if goles == 0:
    print("Sin goles")
elif goles <= 2:
    print("Buen partido")
else:
    print("Gran goleada")
```

---

# 31. Cajero automático

```python
saldo = 1500

if saldo >= 5000:
    print("Cliente Premium")
elif saldo >= 1000:
    print("Cliente Regular")
else:
    print("Saldo bajo")
```

---

# 32. Nivel de videojuego

```python
puntos = 850

if puntos >= 1000:
    print("Experto")
elif puntos >= 500:
    print("Intermedio")
else:
    print("Principiante")
```

---

# 33. Velocidad del internet

```python
mbps = 120

if mbps >= 200:
    print("Muy rápida")
elif mbps >= 100:
    print("Rápida")
else:
    print("Básica")
```

---

# 34. Número de mascotas

```python
mascotas = 2

if mascotas == 0:
    print("Sin mascotas")
elif mascotas <= 2:
    print("Pocas mascotas")
else:
    print("Muchas mascotas")
```

---

# 35. Nivel de ahorro

```python
ahorro = 7000

if ahorro >= 10000:
    print("Excelente ahorro")
elif ahorro >= 5000:
    print("Buen ahorro")
else:
    print("Debe ahorrar más")
```

---

# 36. Clasificación de IMC

```python
imc = 24

if imc < 18.5:
    print("Bajo peso")
elif imc < 25:
    print("Normal")
else:
    print("Sobrepeso")
```

---

# 37. Hora del día

```python
hora = 8

if hora < 12:
    print("Buenos días")
elif hora < 19:
    print("Buenas tardes")
else:
    print("Buenas noches")
```

---

# 38. Estado del examen

```python
calificacion = 100

if calificacion == 100:
    print("Perfecto")
elif calificacion >= 70:
    print("Aprobado")
else:
    print("Reprobado")
```

---

# 39. Tipo de vehículo

```python
ruedas = 2

if ruedas == 2:
    print("Motocicleta")
elif ruedas == 4:
    print("Automóvil")
else:
    print("Otro vehículo")
```

---

# 40. Nivel de agua

```python
nivel = 75

if nivel >= 90:
    print("Lleno")
elif nivel >= 50:
    print("Medio")
else:
    print("Bajo")
```

---

# 41. Precio de boleto

```python
edad = 8

if edad < 12:
    print("Boleto infantil")
elif edad < 60:
    print("Boleto adulto")
else:
    print("Boleto adulto mayor")
```

---

# 42. Desempeño escolar

```python
promedio = 9.5

if promedio >= 9:
    print("Excelente")
elif promedio >= 8:
    print("Bueno")
else:
    print("Regular")
```

---

# 43. Ranking de videojuego

```python
nivel = 50

if nivel >= 100:
    print("Leyenda")
elif nivel >= 50:
    print("Veterano")
else:
    print("Novato")
```

---

# 44. Tipo de cliente

```python
compras = 20

if compras >= 50:
    print("Cliente Oro")
elif compras >= 10:
    print("Cliente Plata")
else:
    print("Cliente Bronce")
```

---

# 45. Rendimiento deportivo

```python
tiempo = 12

if tiempo < 10:
    print("Excelente")
elif tiempo < 15:
    print("Bueno")
else:
    print("Mejorable")
```

---

# 46. Clasificación de película

```python
edad = 17

if edad >= 18:
    print("Clasificación C")
elif edad >= 13:
    print("Clasificación B")
else:
    print("Clasificación A")
```

---

# 47. Tipo de clima

```python
temperatura = 5

if temperatura < 10:
    print("Muy frío")
elif temperatura < 25:
    print("Agradable")
else:
    print("Muy caliente")
```

---

# 48. Calificación de servicio

```python
puntuacion = 4

if puntuacion == 5:
    print("Excelente")
elif puntuacion >= 3:
    print("Bueno")
else:
    print("Malo")
```

---

# 49. Nivel de combustible

```python
litros = 40

if litros >= 50:
    print("Tanque lleno")
elif litros >= 20:
    print("Nivel medio")
else:
    print("Repostar")
```

---

# 50. Estado del proyecto

```python
avance = 85

if avance == 100:
    print("Terminado")
elif avance >= 50:
    print("En proceso")
else:
    print("Iniciado")
```

---

# 51. Comparación de dos números

```python
a = 10
b = 20

if a > b:
    print("A es mayor")
elif a < b:
    print("B es mayor")
else:
    print("Son iguales")
```

---

# 52. Puntaje de examen

```python
puntos = 45

if puntos >= 90:
    print("Sobresaliente")
elif puntos >= 60:
    print("Satisfactorio")
else:
    print("Insuficiente")
```

---

# 53. Estado de conexión

```python
senal = 3

if senal >= 5:
    print("Excelente")
elif senal >= 3:
    print("Aceptable")
else:
    print("Débil")
```

---

# 54. Descuento según edad

```python
edad = 65

if edad < 12:
    print("50% descuento")
elif edad >= 60:
    print("30% descuento")
else:
    print("Sin descuento")
```

---

# 55. Número de materias reprobadas

```python
reprobadas = 1

if reprobadas == 0:
    print("Excelente")
elif reprobadas <= 2:
    print("Regular")
else:
    print("Riesgo académico")
```

---

# 56. Estado del clima

```python
lluvia = 0

if lluvia == 0:
    print("Soleado")
elif lluvia <= 50:
    print("Nublado")
else:
    print("Lluvioso")
```

---

# 57. Rendimiento de batería

```python
porcentaje = 95

if porcentaje >= 90:
    print("Excelente")
elif porcentaje >= 50:
    print("Normal")
else:
    print("Cargar batería")
```

---

# 58. Categoría de peso

```python
peso = 72

if peso < 50:
    print("Ligero")
elif peso < 80:
    print("Medio")
else:
    print("Pesado")
```

---

# 59. Tipo de acceso

```python
rol = "editor"

if rol == "admin":
    print("Control total")
elif rol == "editor":
    print("Puede modificar")
else:
    print("Solo lectura")
```

---

# 60. Evaluación final

```python
promedio = 8.8

if promedio >= 9:
    print("Excelente")
elif promedio >= 8:
    print("Muy bien")
elif promedio >= 7:
    print("Bien")
else:
    print("Debe mejorar")
```

## Actividad para el estudiante

Modifica cada programa para que los datos sean capturados mediante `input()` y prueba diferentes valores para observar cómo cambian los resultados de las estructuras condicionales `if`, `if else` y `elif`. Esto ayudará a comprender la toma de decisiones en Python y el flujo de ejecución de los programas.
