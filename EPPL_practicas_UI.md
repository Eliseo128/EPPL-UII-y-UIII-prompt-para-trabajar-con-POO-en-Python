# Prácticas Python — Unidad I: Fundamentos de Programación Lógica

**Módulo I:** Desarrolla programación lógica para solucionar problemas  
**Submódulo 2:** Elabora proyectos con programación lógica  
**Unidad I:** Fundamentos de programación lógica y entorno de desarrollo  
**Nivel:** Preparatoria — Principiante  
**Lenguaje:** Python  
**Herramientas:** Visual Studio Code, Git y GitHub  

> Todos los ejemplos simulan Inteligencia Artificial utilizando únicamente los fundamentos de la Unidad I: variables, tipos de datos, operadores, lógica secuencial y algoritmos.

---

## Índice

1. [Prácticas Guiadas](#1-prácticas-guiadas)
   - [Guiada 1 — El chatbot que te saluda (ARIA)](#guiada-1--el-chatbot-que-te-saluda-aria)
   - [Guiada 2 — Calculadora Inteligente](#guiada-2--calculadora-inteligente)
   - [Guiada 3 — Detector de Temperatura IA](#guiada-3--detector-de-temperatura-ia)
2. [Prácticas Supervisadas](#2-prácticas-supervisadas)
   - [Supervisada 1 — Generador de Personaje RPG](#supervisada-1--generador-de-personaje-rpg)
   - [Supervisada 2 — Clasificador de Emociones IA](#supervisada-2--clasificador-de-emociones-ia)
3. [Prácticas Autónomas](#3-prácticas-autónomas)
   - [Autónoma 1 — Sistema de Triaje Médico IA](#autónoma-1--sistema-de-triaje-médico-ia)
   - [Autónoma 2 — Crea tu Propio Asistente IA](#autónoma-2--crea-tu-propio-asistente-ia)

---

## 1. Prácticas Guiadas

> **Rol del docente:** Conduce la actividad. Escribe el código en pantalla línea por línea mientras explica cada concepto. El alumno observa, replica y hace preguntas.

---

### Guiada 1 — El chatbot que te saluda (ARIA)

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Guiada |
| **Temas** | Variables, tipos de datos, entrada/salida, f-strings |
| **Fase** | Desarrollo |
| **Evaluación** | Formativa — Prácticas guiadas / Rúbrica |
| **Ponderación** | 10% |

#### Objetivo

Usar variables, `input()` y `print()` para simular que un asistente virtual "aprende" tu nombre y te personaliza una respuesta. El alumno comprenderá cómo la IA conversacional usa datos del usuario para generar respuestas personalizadas.

#### Pasos de la práctica

1. El docente escribe el código en pantalla línea por línea.
2. El alumno copia y ejecuta en VS Code, observando la salida en la terminal.
3. El docente explica cada variable, su nombre, tipo de dato asignado y la conversión con `int()`.
4. Se discute: ¿por qué una IA necesita guardar datos del usuario en variables?

#### Código Python

```python
# Práctica Guiada 1 — Asistente Virtual "ARIA"
# Tema: Variables, tipos de datos, entrada y salida
# Nivel: Principiante — Preparatoria

print("=" * 40)
print("  Bienvenido a ARIA — Asistente IA  ")
print("=" * 40)

# Captura de datos del usuario (tipo str)
nombre = input("¿Cómo te llamas? ")
ciudad = input("¿En qué ciudad vives? ")

# Captura de dato numérico (tipo int mediante conversión)
edad = int(input("¿Cuántos años tienes? "))

# Cálculo con operador aritmético
anio_nacimiento = 2025 - edad

# Salida personalizada con f-strings
print(f"\nHola, {nombre}! 👋")
print(f"Vives en {ciudad} y naciste en {anio_nacimiento}.")
print(f"Dato curioso: en 10 años tendrás {edad + 10} años.")
print("\nARIA lista para ayudarte. 🤖")
```

#### Salida esperada

```
========================================
  Bienvenido a ARIA — Asistente IA
========================================
¿Cómo te llamas? Ana
¿En qué ciudad vives? Juárez
¿Cuántos años tienes? 16

Hola, Ana! 👋
Vives en Juárez y naciste en 2009.
Dato curioso: en 10 años tendrás 26 años.

ARIA lista para ayudarte. 🤖
```

#### Conceptos clave que el docente debe reforzar

- **Variable:** contenedor con nombre que guarda un valor (`nombre = "Ana"`).
- **Tipo `str`:** cadena de texto, resultado de `input()` siempre es `str`.
- **Tipo `int`:** número entero; se convierte con `int()`.
- **f-string:** forma moderna de insertar variables dentro de un texto: `f"Hola, {nombre}"`.
- **Operador aritmético `-`:** se aplica directamente sobre variables numéricas.

#### Preguntas de reflexión para el grupo

- ¿Qué pasaría si no convertimos la edad a `int`?
- ¿Cómo crees que los asistentes como Siri o Alexa guardan tu nombre?

---

### Guiada 2 — Calculadora Inteligente

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Guiada |
| **Temas** | Operadores aritméticos, lógicos y relacionales |
| **Fase** | Desarrollo |
| **Evaluación** | Formativa — Ejercicios resueltos / Lista de cotejo |
| **Ponderación** | 10% |

#### Objetivo

Aplicar los tres tipos de operadores (aritméticos, relacionales y lógicos) para construir una mini calculadora que "razona" sobre los resultados, simulando el análisis que hace una IA al procesar datos numéricos.

#### Pasos de la práctica

1. El docente ejecuta el programa proyectando distintas entradas al grupo.
2. Los alumnos **predicen el resultado** en voz alta antes de que el programa lo muestre.
3. Se discuten en detalle los operadores `//` (división entera) y `%` (módulo) con ejemplos cotidianos.
4. El docente explica el operador ternario `a if condición else b`.

#### Código Python

```python
# Práctica Guiada 2 — Calculadora con "razonamiento"
# Tema: Operadores aritméticos, lógicos y relacionales
# Nivel: Principiante — Preparatoria

print("🤖 Calculadora IA — Ingresa dos números")

# Captura con conversión a flotante
a = float(input("Número A: "))
b = float(input("Número B: "))

# --- Operadores aritméticos ---
print(f"\n📊 Resultados aritméticos:")
print(f"  Suma:              {a} + {b} = {a + b}")
print(f"  Resta:             {a} - {b} = {a - b}")
print(f"  Multiplicación:    {a} × {b} = {a * b}")
print(f"  División:          {a} ÷ {b} = {a / b:.2f}")
print(f"  División entera:   {a} // {b} = {a // b}")
print(f"  Módulo (resto):    {a} % {b} = {a % b}")
print(f"  Potencia:          {a} ^ {b} = {a ** b:.2f}")

# --- Operadores relacionales ---
print(f"\n🔍 Comparaciones (resultado True o False):")
print(f"  ¿A es mayor que B?      {a > b}")
print(f"  ¿A es menor que B?      {a < b}")
print(f"  ¿Son iguales?           {a == b}")
print(f"  ¿Son diferentes?        {a != b}")
print(f"  ¿A es mayor o igual?    {a >= b}")

# --- Operadores lógicos ---
positivos = a > 0 and b > 0
alguno_positivo = a > 0 or b > 0
print(f"\n🧠 Lógica booleana:")
print(f"  ¿Ambos son positivos?   {positivos}")
print(f"  ¿Al menos uno positivo? {alguno_positivo}")

# --- Razonamiento simple (operador ternario) ---
mayor = a if a > b else b
menor = a if a < b else b
print(f"\n✅ Análisis IA:")
print(f"  El número mayor es: {mayor}")
print(f"  El número menor es: {menor}")
print(f"  Su promedio es:     {(a + b) / 2:.2f}")
```

#### Salida esperada (ejemplo con A=8, B=3)

```
🤖 Calculadora IA — Ingresa dos números
Número A: 8
Número B: 3

📊 Resultados aritméticos:
  Suma:              8.0 + 3.0 = 11.0
  Resta:             8.0 - 3.0 = 5.0
  Multiplicación:    8.0 × 3.0 = 24.0
  División:          8.0 ÷ 3.0 = 2.67
  División entera:   8.0 // 3.0 = 2.0
  Módulo (resto):    8.0 % 3.0 = 2.0
  Potencia:          8.0 ^ 3.0 = 512.00

🔍 Comparaciones (resultado True o False):
  ¿A es mayor que B?      True
  ¿A es menor que B?      False
  ¿Son iguales?           False
  ¿Son diferentes?        True
  ¿A es mayor o igual?    True

🧠 Lógica booleana:
  ¿Ambos son positivos?   True
  ¿Al menos uno positivo? True

✅ Análisis IA:
  El número mayor es: 8.0
  El número menor es: 3.0
  Su promedio es:     5.50
```

#### Reto docente

> Pide a los alumnos que predigan qué sucede si `b = 0`. Ejecuten el programa y observen el error `ZeroDivisionError`. Discute: ¿cómo una IA real maneja errores en los datos de entrada?

#### Ejemplos cotidianos del operador módulo `%`

| Uso | Código | Resultado |
|---|---|---|
| ¿Es par o impar? | `numero % 2 == 0` | `True` si es par |
| ¿Es múltiplo de 5? | `numero % 5 == 0` | `True` si es múltiplo |
| Minutos restantes | `135 % 60` | `15` minutos |

---

### Guiada 3 — Detector de Temperatura IA

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Guiada |
| **Temas** | Algoritmos, pseudocódigo, diagramas de flujo, lógica secuencial |
| **Fase** | Desarrollo |
| **Evaluación** | Formativa — Diagramas y pseudocódigos / Rúbrica |
| **Ponderación** | 15% |

#### Objetivo

Diseñar primero el algoritmo en pseudocódigo (como lo hace un programador profesional), luego traducirlo a Python línea a línea. El alumno comprenderá que la IA sigue reglas lógicas definidas por un algoritmo.

#### Pasos de la práctica

1. El docente escribe el **pseudocódigo** en el pizarrón antes de abrir VS Code.
2. Juntos (docente + grupo) traducen el pseudocódigo a Python, línea por línea.
3. Se ejecuta el programa y se compara la salida con el pseudocódigo original.
4. El docente conecta el ejercicio con el concepto de **diagrama de flujo** (estructura `SI/SINO`).

#### Pseudocódigo (escribir en pizarrón ANTES de programar)

```
INICIO
  MOSTRAR "Sistema Sensor IA"
  LEER temperatura
  
  SI temperatura < 0 ENTONCES
    estado ← "CONGELAMIENTO — Alerta crítica"
    consejo ← "No salgas sin ropa térmica"
  SINO SI temperatura < 18 ENTONCES
    estado ← "Frío — Temperatura baja"
    consejo ← "Se recomienda abrigo"
  SINO SI temperatura < 30 ENTONCES
    estado ← "Normal — Condiciones ideales"
    consejo ← "Clima agradable para actividades"
  SINO
    estado ← "CALOR EXTREMO — Alerta IA"
    consejo ← "Mantente hidratado y en sombra"
  FIN SI
  
  MOSTRAR temperatura, estado, consejo
FIN
```

#### Código Python

```python
# Práctica Guiada 3 — Sensor de Temperatura con Lógica IA
# Tema: Algoritmos, pseudocódigo, diagramas de flujo, lógica secuencial
# Nivel: Principiante — Preparatoria
#
# INSTRUCCIÓN: Este código debe programarse DESPUÉS de escribir
# el pseudocódigo en el pizarrón. No al revés.

print("🌡️  Sistema Sensor IA — Monitor Ambiental")
print("-" * 45)

# Entrada de dato con conversión a float
temp = float(input("Ingresa la temperatura actual (°C): "))

# Estructura de decisión — traducción directa del pseudocódigo
if temp < 0:
    estado  = "🔵 CONGELAMIENTO — Alerta crítica"
    consejo = "No salgas sin ropa térmica."
elif temp < 18:
    estado  = "❄️  Frío — Temperatura baja"
    consejo = "Se recomienda abrigo."
elif temp < 30:
    estado  = "✅ Normal — Condiciones ideales"
    consejo = "Clima agradable para actividades."
else:
    estado  = "🔴 CALOR EXTREMO — Alerta IA"
    consejo = "Mantente hidratado y en sombra."

# Reporte de salida
print(f"\nTemperatura registrada: {temp}°C")
print(f"Estado del sistema:     {estado}")
print(f"Recomendación IA:       {consejo}")
```

#### Salida esperada (ejemplo con 35°C)

```
🌡️  Sistema Sensor IA — Monitor Ambiental
---------------------------------------------
Ingresa la temperatura actual (°C): 35

Temperatura registrada: 35.0°C
Estado del sistema:     🔴 CALOR EXTREMO — Alerta IA
Recomendación IA:       Mantente hidratado y en sombra.
```

#### Casos de prueba sugeridos

| Temperatura | Estado esperado |
|---|---|
| -5°C | 🔵 CONGELAMIENTO |
| 10°C | ❄️ Frío |
| 24°C | ✅ Normal |
| 40°C | 🔴 CALOR EXTREMO |

#### Conexión con diagrama de flujo

El docente debe dibujar en el pizarrón los símbolos correspondientes:

- **Óvalo** → INICIO / FIN
- **Paralelogramo** → LEER temperatura / MOSTRAR resultados
- **Rombo** → Condiciones `SI temperatura < 0`, etc.
- **Rectángulo** → Asignación de `estado` y `consejo`

---

## 2. Prácticas Supervisadas

> **Rol del docente:** Observa, orienta y supervisa sin dar la respuesta directa. El alumno trabaja de forma semi-independiente. El docente responde preguntas y evalúa el proceso con guía de observación.

---

### Supervisada 1 — Generador de Personaje RPG

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Supervisada |
| **Temas** | Variables, tipos de datos, conversión, operadores, Git y GitHub |
| **Fase** | Desarrollo |
| **Evaluación** | Formativa — Repositorio funcional / Lista de cotejo |
| **Ponderación** | 10% |

#### Objetivo

Crear un programa completo con variables de distintos tipos de datos y operadores, y subirlo a GitHub realizando el **primer commit real** del proyecto del alumno.

#### Pasos de la práctica

1. El alumno **lee el código completo** antes de escribirlo (no se permite copiar/pegar).
2. Lo escribe manualmente en VS Code y ejecuta, corrigiendo errores con mínima ayuda del docente.
3. Una vez funcional, realiza la secuencia Git completa:
   - `git init`
   - `git add practica_rpg.py`
   - `git commit -m "feat: generador de personaje RPG"`
   - `git push origin main`

#### Código Python

```python
# Práctica Supervisada 1 — Generador de Personaje RPG
# Tema: Variables, tipos de datos, conversión, operadores, Git
# Nivel: Principiante — Preparatoria
# Instrucción: Escribe el código a mano, NO copies y pegues.

print("⚔️  CREADOR DE PERSONAJE — IA Dungeon v1.0")
print("-" * 45)

# --- Captura de datos (tipo str) ---
nombre = input("Nombre del héroe: ")
clase  = input("Clase (Mago / Guerrero / Arquero): ")

# --- Captura de dato numérico (tipo int) ---
nivel  = int(input("Nivel inicial (1-10): "))

# --- Cálculo automático de atributos por nivel ---
# Operadores aritméticos: multiplicación
vida    = nivel * 50
mana    = nivel * 30
ataque  = nivel * 15
defensa = nivel * 10

# --- Bonus especial por clase ---
# Operador: comparación de strings con .lower() para ignorar mayúsculas
if clase.lower() == "mago":
    mana   = int(mana * 1.5)          # Conversión float → int
    bonus  = "✨ +50% Mana por clase Mago"
elif clase.lower() == "guerrero":
    vida   = int(vida * 1.4)
    bonus  = "🛡️  +40% Vida por clase Guerrero"
else:
    ataque = int(ataque * 1.3)
    bonus  = "🏹 +30% Ataque por clase Arquero"

# --- Ficha del personaje generada por IA ---
print(f"\n{'=' * 45}")
print(f"  🧙 FICHA DE PERSONAJE — IA GENERADA")
print(f"{'=' * 45}")
print(f"  Nombre:   {nombre.upper()}")          # str.upper() convierte a mayúsculas
print(f"  Clase:    {clase.capitalize()}")       # str.capitalize() primera letra mayúscula
print(f"  Nivel:    {nivel}")
print(f"  ❤️  Vida:    {vida} HP")
print(f"  💙 Mana:    {mana} MP")
print(f"  ⚔️  Ataque:  {ataque}")
print(f"  🛡️  Defensa: {defensa}")
print(f"  🌟 Bonus:   {bonus}")
print(f"{'=' * 45}")
print("\nPersonaje listo. ¡Que comience la aventura!")
```

#### Salida esperada (ejemplo: Mago nivel 5)

```
⚔️  CREADOR DE PERSONAJE — IA Dungeon v1.0
---------------------------------------------
Nombre del héroe: Zara
Clase (Mago / Guerrero / Arquero): mago
Nivel inicial (1-10): 5

=============================================
  🧙 FICHA DE PERSONAJE — IA GENERADA
=============================================
  Nombre:   ZARA
  Clase:    Mago
  Nivel:    5
  ❤️  Vida:    250 HP
  💙 Mana:    225 MP
  ⚔️  Ataque:  75
  🛡️  Defensa: 50
  🌟 Bonus:   ✨ +50% Mana por clase Mago
=============================================

Personaje listo. ¡Que comience la aventura!
```

#### Lista de cotejo Git — Evaluación del repositorio

| Criterio | Sí | No |
|---|---|---|
| Creó repositorio local con `git init` | | |
| Ejecutó `git add` correctamente | | |
| El mensaje del commit es descriptivo | | |
| Subió el archivo a GitHub con `git push` | | |
| El repositorio es visible en GitHub | | |
| El archivo `.py` ejecuta sin errores | | |

#### Comandos Git completos para el alumno

```bash
# En la terminal integrada de VS Code:
git init
git add practica_rpg.py
git commit -m "feat: generador de personaje RPG"
git branch -M main
git remote add origin https://github.com/tu-usuario/tu-repositorio.git
git push -u origin main
```

---

### Supervisada 2 — Clasificador de Emociones IA

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Supervisada |
| **Temas** | Lógica secuencial, operadores relacionales y lógicos, promedio ponderado |
| **Fase** | Desarrollo |
| **Evaluación** | Formativa — Actividades prácticas / Guía de observación |
| **Ponderación** | 10% |

#### Objetivo

Simular un clasificador de bienestar emocional (como los que realmente usa la IA en aplicaciones de salud mental) usando lógica secuencial, operadores y un cálculo de puntaje ponderado. El alumno trabaja de forma semi-independiente.

#### Pasos de la práctica

1. El alumno diseña primero el **pseudocódigo en papel** antes de abrir VS Code.
2. Escribe el programa completo; el docente supervisa sin dar la respuesta directa.
3. Prueba el programa con al menos **5 combinaciones distintas** y anota los resultados en tabla.
4. Reflexiona: ¿en qué se parece esto a cómo funciona una IA real de análisis emocional?

#### Código Python

```python
# Práctica Supervisada 2 — Clasificador de Emociones IA
# Tema: Lógica secuencial, operadores lógicos y relacionales
# Nivel: Principiante — Preparatoria
# Instrucción: Diseña el pseudocódigo en papel ANTES de programar.

print("🔮 ANÁLISIS DE BIENESTAR — Sistema IA")
print("=" * 45)
print("Responde cada pregunta del 1 (muy malo)")
print("al 10 (excelente)\n")

# --- Entrada de datos (tipo int) ---
animo   = int(input("¿Cómo está tu ánimo hoy?     (1-10): "))
energia = int(input("¿Cuál es tu nivel de energía? (1-10): "))
estres  = int(input("¿Cuánto estrés sientes?        (1-10): "))

# --- Cálculo del puntaje de bienestar (promedio ponderado) ---
# El estrés se invierte: (10 - estres) porque más estrés = peor bienestar
bienestar = (animo * 0.40) + (energia * 0.35) + ((10 - estres) * 0.25)

# --- Clasificación por rangos (lógica secuencial) ---
if bienestar >= 8:
    emocion = "😄 Excelente"
    mensaje = "¡Hoy es un gran día! Aprovéchalo al máximo."
    color   = "VERDE"
elif bienestar >= 6:
    emocion = "🙂 Bien"
    mensaje = "Vas bien. Mantén el ritmo y cuídate."
    color   = "AMARILLO"
elif bienestar >= 4:
    emocion = "😐 Regular"
    mensaje = "Considera tomar un descanso hoy."
    color   = "NARANJA"
else:
    emocion = "😔 Necesitas apoyo"
    mensaje = "Habla con alguien de confianza. ¡No estás solo!"
    color   = "ROJO"

# --- Reporte generado ---
print(f"\n{'=' * 45}")
print(f"  REPORTE IA — ANÁLISIS DE BIENESTAR")
print(f"{'=' * 45}")
print(f"  Ánimo:             {animo}/10")
print(f"  Energía:           {energia}/10")
print(f"  Estrés:            {estres}/10")
print(f"  Puntaje bienestar: {bienestar:.1f}/10")
print(f"  Nivel de alerta:   {color}")
print(f"  Estado emocional:  {emocion}")
print(f"  Recomendación:     {mensaje}")
print(f"{'=' * 45}")
print("\n⚠️  Sistema educativo — no reemplaza orientación profesional.")
```

#### Tabla de registro para el alumno (5 pruebas)

| Prueba | Ánimo | Energía | Estrés | Puntaje | Resultado |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

#### Preguntas de análisis

- ¿Por qué se invierte el valor del estrés con `(10 - estres)`?
- ¿Qué significa que el ánimo tenga un peso de `0.40` y el estrés de `0.25`?
- ¿Cómo podría mejorarse este clasificador con más preguntas?

---

## 3. Prácticas Autónomas

> **Rol del docente:** Evaluador. El alumno trabaja de forma completamente independiente. El docente solo aclara dudas conceptuales, no da código. Se evalúa con rúbrica analítica.

---

### Autónoma 1 — Sistema de Triaje Médico IA

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Autónoma — Proyecto Integrador |
| **Temas** | Todos los temas de la Unidad I |
| **Fase** | Cierre |
| **Evaluación** | Sumativa — Proyecto básico funcional / Rúbrica analítica |
| **Ponderación** | 20% |

#### Objetivo

Aplicar de forma autónoma y articulada todos los contenidos de la unidad: variables, tipos de datos, operadores, algoritmos, pseudocódigo, diagrama de flujo y lógica secuencial. El alumno simula un sistema real de clasificación de urgencias médicas (triage), y lo sube a GitHub con documentación básica.

#### Pasos de la práctica

1. El alumno diseña el **pseudocódigo** en papel — el docente lo revisa y aprueba **antes** de que el alumno abra VS Code.
2. El alumno dibuja el **diagrama de flujo** correspondiente.
3. Programa la solución completamente solo en VS Code.
4. Prueba el programa con al menos **6 casos distintos** (incluyendo casos límite).
5. Sube a GitHub con un `README.md` que explique qué hace el programa.

#### Pseudocódigo que el alumno debe elaborar (referencia para el docente)

```
INICIO
  MOSTRAR encabezado del sistema
  
  LEER paciente (str)
  LEER edad (int)
  LEER temperatura (float)
  LEER presion (int)
  LEER dolor (int, escala 1-10)
  
  puntos ← 0
  
  SI temperatura >= 39.5 O temperatura < 35 ENTONCES
    puntos ← puntos + 3
  SINO SI temperatura >= 38 ENTONCES
    puntos ← puntos + 2
  FIN SI
  
  SI presion > 160 O presion < 90 ENTONCES
    puntos ← puntos + 3
  SINO SI presion > 140 ENTONCES
    puntos ← puntos + 1
  FIN SI
  
  SI dolor >= 8 ENTONCES
    puntos ← puntos + 3
  SINO SI dolor >= 5 ENTONCES
    puntos ← puntos + 2
  SINO
    puntos ← puntos + 1
  FIN SI
  
  SI edad < 5 O edad > 70 ENTONCES
    puntos ← puntos + 2
  FIN SI
  
  SI puntos >= 8 ENTONCES
    nivel ← "ROJO — Emergencia inmediata"
    tiempo ← "Menos de 5 minutos"
  SINO SI puntos >= 5 ENTONCES
    nivel ← "NARANJA — Urgencia alta"
    tiempo ← "Menos de 30 minutos"
  SINO SI puntos >= 3 ENTONCES
    nivel ← "AMARILLO — Urgencia media"
    tiempo ← "Menos de 2 horas"
  SINO
    nivel ← "VERDE — No urgente"
    tiempo ← "Atención programada"
  FIN SI
  
  MOSTRAR reporte completo del paciente
FIN
```

#### Código Python (referencia para el docente — no mostrar al alumno)

```python
# Práctica Autónoma 1 — Triaje Médico Inteligente
# PROYECTO INTEGRADOR — Unidad I
# Nivel: Principiante — Preparatoria
#
# IMPORTANTE: El alumno debe haber diseñado y entregado
# pseudocódigo y diagrama de flujo ANTES de programar.

print("🏥 SISTEMA DE TRIAJE IA — Hospital Virtual")
print("=" * 50)
print("Sistema basado en inteligencia artificial")
print("para clasificar urgencias médicas")
print()

# === MÓDULO 1: CAPTURA DE DATOS DEL PACIENTE ===
# Tipos de datos: str, int, float, int, int
paciente    = input("Nombre del paciente: ")
edad        = int(input("Edad: "))
temperatura = float(input("Temperatura corporal (°C): "))
presion     = int(input("Presión sistólica (mmHg): "))
dolor       = int(input("Nivel de dolor (1-10): "))

# === MÓDULO 2: ALGORITMO DE CLASIFICACIÓN IA ===
# Sistema de puntos: mayor puntaje = mayor urgencia
puntos = 0

# Factor temperatura (°C)
if temperatura >= 39.5 or temperatura < 35:
    puntos += 3          # Fiebre alta o hipotermia: crítico
elif temperatura >= 38:
    puntos += 2          # Fiebre moderada
# Entre 35 y 37.9 = normal, no suma puntos

# Factor presión arterial (mmHg)
if presion > 160 or presion < 90:
    puntos += 3          # Hipertensión severa o hipotensión: crítico
elif presion > 140:
    puntos += 1          # Hipertensión moderada

# Factor dolor (escala 1-10)
if dolor >= 8:
    puntos += 3          # Dolor severo
elif dolor >= 5:
    puntos += 2          # Dolor moderado
else:
    puntos += 1          # Dolor leve

# Factor edad vulnerable
if edad < 5 or edad > 70:
    puntos += 2          # Niños pequeños y adultos mayores: riesgo adicional

# === MÓDULO 3: CLASIFICACIÓN FINAL ===
if puntos >= 8:
    nivel    = "🔴 ROJO — Emergencia inmediata"
    tiempo   = "Atención en menos de 5 minutos"
elif puntos >= 5:
    nivel    = "🟠 NARANJA — Urgencia alta"
    tiempo   = "Atención en menos de 30 minutos"
elif puntos >= 3:
    nivel    = "🟡 AMARILLO — Urgencia media"
    tiempo   = "Atención en menos de 2 horas"
else:
    nivel    = "🟢 VERDE — No urgente"
    tiempo   = "Atención programada"

# === MÓDULO 4: REPORTE GENERADO POR IA ===
print(f"\n{'=' * 50}")
print(f"  REPORTE GENERADO — SISTEMA IA TRIAJE")
print(f"{'=' * 50}")
print(f"  Paciente:      {paciente.title()}, {edad} años")
print(f"  Temperatura:   {temperatura}°C")
print(f"  Presión:       {presion} mmHg")
print(f"  Dolor:         {dolor}/10")
print(f"  Puntaje IA:    {puntos} puntos de riesgo")
print(f"  Clasificación: {nivel}")
print(f"  Tiempo espera: {tiempo}")
print(f"{'=' * 50}")
print()
print("⚠️  Este sistema es educativo, no reemplaza diagnóstico médico real.")
```

#### Casos de prueba obligatorios

| # | Datos de entrada | Resultado esperado |
|---|---|---|
| 1 | 35 años, 40.0°C, 170 mmHg, dolor 9 | 🔴 ROJO |
| 2 | 80 años, 37.0°C, 145 mmHg, dolor 6 | 🟠 NARANJA |
| 3 | 25 años, 38.5°C, 130 mmHg, dolor 5 | 🟡 AMARILLO |
| 4 | 20 años, 36.5°C, 120 mmHg, dolor 2 | 🟢 VERDE |
| 5 | 3 años, 37.5°C, 95 mmHg, dolor 3 | (variable — analizar) |
| 6 | 75 años, 34.5°C, 85 mmHg, dolor 7 | 🔴 ROJO |

#### Entregables para evaluación con rúbrica analítica

| # | Entregable | Instrumento |
|---|---|---|
| 1 | Pseudocódigo manuscrito | Rúbrica — Secuencia lógica |
| 2 | Diagrama de flujo (papel o digital) | Rúbrica — Uso de símbolos |
| 3 | Archivo `triaje_ia.py` funcional | Rúbrica — Solución del problema |
| 4 | Repositorio GitHub con commit descriptivo | Lista de cotejo — Git |
| 5 | Archivo `README.md` con descripción del programa | Rúbrica — Organización |

#### Rúbrica analítica — Sistema de Triaje IA

| Criterio | Excelente (4) | Bueno (3) | Regular (2) | Insuficiente (1) |
|---|---|---|---|---|
| **Pseudocódigo** | Completo, secuencial, sin errores lógicos | Mínimos errores de lógica | Tiene errores pero estructura visible | Incompleto o ausente |
| **Diagrama de flujo** | Símbolos correctos, flujo claro | Algunos errores de símbolo | Uso limitado de símbolos | Incorrecto o ausente |
| **Código Python** | Ejecuta sin errores, todos los casos correctos | 1-2 errores menores | Ejecuta parcialmente | No ejecuta |
| **Variables y tipos** | Usa str, int, float correctamente | Usa 2 tipos correctamente | Usa solo 1 tipo | No diferencia tipos |
| **Operadores** | Usa aritméticos, relacionales y lógicos | Usa 2 tipos de operadores | Solo operadores básicos | Sin operadores correctos |
| **Git / GitHub** | Commit descriptivo, repositorio público visible | Repositorio creado, commit simple | Repositorio creado sin commit | No entregó en GitHub |
| **README.md** | Describe el programa, instrucciones de uso | Descripción básica presente | Solo nombre del archivo | Ausente |

---

### Autónoma 2 — Crea tu Propio Asistente IA

| Campo | Detalle |
|---|---|
| **Tipo** | Práctica Autónoma — Reto Creativo |
| **Temas** | Todos los temas de la Unidad I — Aplicación libre |
| **Fase** | Cierre |
| **Evaluación** | Sumativa — Autoevaluación y coevaluación / Escala estimativa |
| **Ponderación** | 5% |

#### Objetivo

El alumno elige un problema real de su contexto cotidiano y diseña su propio "asistente IA" desde cero, demostrando dominio autónomo de todos los contenidos de la unidad. No existe una solución única ni correcta.

#### Pasos de la práctica

1. El alumno elige un problema de su vida cotidiana (ver ideas abajo).
2. Diseña pseudocódigo y diagrama de flujo; el docente **aprueba el diseño** antes de que programe.
3. Programa la solución completamente solo en VS Code.
4. Prueba con mínimo **5 casos distintos** incluyendo casos límite.
5. Sube a GitHub con `README.md` que incluya: nombre del asistente, problema que resuelve, instrucciones de uso.
6. Presenta el programa al grupo (2-3 minutos): explica el problema, muestra el diagrama de flujo y ejecuta el programa en vivo.

#### Plantilla de inicio (el alumno la adapta a su proyecto)

```python
# ============================================
# Mi Asistente IA Personal
# ============================================
# Nombre del alumno:
# Nombre del asistente:
# Problema que resuelve:
# Fecha:
# ============================================

print("🤖 [NOMBRE DE TU ASISTENTE]")
print("[Descripción breve de lo que hace]")
print("-" * 40)

# --- PASO 1: Captura al menos 3 datos del usuario ---
# Usa al menos un str, un int y un float
variable1 = input("[Pregunta 1 — dato str]: ")
variable2 = int(input("[Pregunta 2 — dato int]: "))
variable3 = float(input("[Pregunta 3 — dato float]: "))

# --- PASO 2: Realiza al menos 2 cálculos con operadores ---
resultado1 = 0   # Reemplaza con tu cálculo
resultado2 = 0   # Reemplaza con tu cálculo

# --- PASO 3: Clasifica con al menos 3 condiciones ---
if resultado1 > 0:           # Tu condición real aquí
    respuesta = "[Caso 1 — describe la situación]"
elif resultado1 > -1:        # Tu condición real aquí
    respuesta = "[Caso 2 — describe la situación]"
else:
    respuesta = "[Caso 3 — describe la situación]"

# --- PASO 4: Muestra un reporte claro y organizado ---
print(f"\n--- ANÁLISIS DE TU ASISTENTE IA ---")
print(f"[Tu reporte personalizado aquí]")
print(f"Resultado: {respuesta}")
```

#### Requisitos mínimos del programa

| Requisito | Descripción |
|---|---|
| Variables | Mínimo 3 variables con nombres descriptivos |
| Tipos de datos | Usar str, int y float (al menos uno de cada tipo) |
| Operadores | Usar operadores aritméticos Y relacionales |
| Lógica | Mínimo 3 condiciones (`if / elif / else`) |
| Entrada/Salida | `input()` para captura, `print()` con f-strings para reporte |
| Documentación | Comentarios en el código que expliquen cada sección |
| Git | Repositorio en GitHub con `README.md` |

#### Ideas de asistentes IA para elegir

| Idea | Problema que resuelve |
|---|---|
| 🎓 Orientador vocacional | Recomienda área de estudio según habilidades e intereses |
| 💪 Asesor deportivo | Calcula IMC y recomienda actividad física |
| 🎵 DJ IA | Recomienda género musical según estado de ánimo |
| 💰 Gestor de mesada | Clasifica si el gasto semanal es excesivo o adecuado |
| 🌱 Consejero ambiental | Calcula huella de carbono de actividades cotidianas |
| 🏫 Calculador de promedio | Analiza calificaciones y recomienda áreas de mejora |
| 🍕 Recomendador de comida | Sugiere qué comer según calorías y presupuesto |
| 🚦 Semáforo de productividad | Evalúa hábitos de estudio y clasifica rendimiento |

#### Escala estimativa — Autoevaluación del alumno

| Indicador | Excelente | Bueno | Regular | Deficiente |
|---|---|---|---|---|
| Elegí un problema real y relevante | | | | |
| Diseñé el pseudocódigo antes de programar | | | | |
| Usé correctamente los tipos de datos | | | | |
| Mis condiciones resuelven el problema | | | | |
| El código tiene comentarios claros | | | | |
| Subí el proyecto a GitHub con README | | | | |
| Probé el programa con múltiples casos | | | | |
| Puedo explicar mi programa al grupo | | | | |

#### Escala estimativa — Coevaluación (compañero evalúa compañero)

| Indicador | Sí | Parcialmente | No |
|---|---|---|---|
| El programa ejecuta sin errores | | | |
| La salida es clara y comprensible | | | |
| El problema elegido es creativo y útil | | | |
| La presentación fue clara y ordenada | | | |
| El repositorio de GitHub es visible | | | |

---

## Resumen de Evaluación — Unidad I

| Práctica | Tipo | Fase | Instrumento | Ponderación |
|---|---|---|---|---|
| Guiada 1 — ARIA | Diagnóstica/Formativa | Apertura | Lista de cotejo | 5% |
| Guiada 2 — Calculadora | Formativa | Desarrollo | Lista de cotejo | 10% |
| Guiada 3 — Temperatura | Formativa | Desarrollo | Rúbrica | 15% |
| Supervisada 1 — RPG + Git | Formativa | Desarrollo | Lista de cotejo | 10% |
| Supervisada 2 — Emociones | Formativa | Desarrollo | Guía de observación | 10% |
| Autónoma 1 — Triaje IA | Sumativa | Cierre | Rúbrica analítica | 20% |
| Autónoma 2 — Asistente libre | Sumativa | Cierre | Escala estimativa | 5% |
| **Total prácticas** | | | | **75%** |

> El 25% restante corresponde al cuestionario diagnóstico (5%) y actividades de algoritmia previas (20%) según la planeación didáctica original.

---

## Notas para el Docente

- **Orden de las prácticas:** Siempre respetar la progresión Guiada → Supervisada → Autónoma. No saltar etapas.
- **Pseudocódigo primero:** En todas las prácticas de algoritmos, el pseudocódigo en papel es un requisito previo a abrir VS Code.
- **Git desde la Supervisada 1:** Integrar Git desde la primera práctica supervisada para que los alumnos lo practiquen de forma natural.
- **Simulación de IA:** Todos los ejemplos usan lógica que los alumnos pueden entender y modificar. El objetivo es que vean la conexión entre los fundamentos y las aplicaciones reales de IA.
- **Errores como aprendizaje:** Cuando los alumnos generen errores (`TypeError`, `ZeroDivisionError`, `ValueError`), aprovecharlos como momentos de aprendizaje sobre validación de datos en sistemas de IA.

---

*Documento generado para: Módulo I — Submódulo 2 — Unidad I*  
*Nivel: Preparatoria — Principiante | Lenguaje: Python | Herramientas: VS Code, Git, GitHub*
