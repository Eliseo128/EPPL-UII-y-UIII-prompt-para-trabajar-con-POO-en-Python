Aquí tienes los **60 ejercicios con su pseudocódigo correspondiente**, numerados y alineados exactamente con la redacción solicitada. He utilizado una notación pseudocódigo estándar (compatible con PSeInt, algoritmos académicos o lógica estructurada) para que sea fácil de trasladar a cualquier lenguaje de programación.

---

### Ejercicio 1
**Enunciado:** Crea una aplicación que pida un número y calcule su factorial.
```pseudocode
Algoritmo Factorial
    Definir num, i, resultado como Entero
    Escribir "Ingrese un número:"
    Leer num
    resultado <- 1
    Para i <- 1 Hasta num Hacer
        resultado <- resultado * i
    FinPara
    Escribir "El factorial de ", num, " es: ", resultado
FinAlgoritmo
```

### Ejercicio 2
**Enunciado:** Adivinar un número (1-100) con 10 intentos, indicando mayor/menor y restantes.
```pseudocode
Algoritmo AdivinarNumero
    Definir objetivo, intento, restantes como Entero
    objetivo <- Aleatorio(1, 100)
    restantes <- 10
    Repetir
        Escribir "Intenta adivinar (restantes: ", restantes, "):"
        Leer intento
        restantes <- restantes - 1
        Si intento < objetivo Entonces Escribir "Es MAYOR."
        Sino Si intento > objetivo Entonces Escribir "Es MENOR."
        FinSi
    Hasta Que (intento = objetivo) O (restantes = 0)
    Si intento = objetivo Entonces Escribir "¡Acertaste en ", 10-restantes, " intentos!"
    Sino Escribir "Fin de intentos. El número era: ", objetivo
    FinSi
FinAlgoritmo
```

### Ejercicio 3
**Enunciado:** Pedir números hasta 0. Imprimir suma y media.
```pseudocode
Algoritmo SumaMedia
    Definir num, suma, contador como Real
    suma <- 0; contador <- 0
    Repetir
        Escribir "Número (0 para terminar):"
        Leer num
        Si num <> 0 Entonces suma <- suma + num; contador <- contador + 1
        FinSi
    Hasta Que num = 0
    Si contador > 0 Entonces Escribir "Suma: ", suma, " | Media: ", suma/contador
    Sino Escribir "No se ingresaron datos."
    FinSi
FinAlgoritmo
```

### Ejercicio 4
**Enunciado:** Pedir cantidad de números. Contar >0, <0, =0.
```pseudocode
Algoritmo ContarSignos
    Definir cant, i, num, pos, neg, cero como Entero
    Escribir "¿Cuántos números?"
    Leer cant
    pos <- 0; neg <- 0; cero <- 0
    Para i <- 1 Hasta cant Hacer
        Leer num
        Si num > 0 Entonces pos <- pos + 1
        Sino Si num < 0 Entonces neg <- neg + 1
        Sino cero <- cero + 1
        FinSi
    FinPara
    Escribir "Pos: ", pos, " | Neg: ", neg, " | Cero: ", cero
FinAlgoritmo
```

### Ejercicio 5
**Enunciado:** Pedir caracteres, indicar VOCAL/NO VOCAL hasta espacio.
```pseudocode
Algoritmo Vocales
    Definir car como Caracter
    Repetir
        Escribir "Carácter:"
        Leer car
        Si car = ' ' Entonces Salir
        FinSi
        Si car EN ['a','e','i','o','u','A','E','I','O','U'] Entonces Escribir "VOCAL"
        Sino Escribir "NO VOCAL"
        FinSi
    Hasta Que Falso
FinAlgoritmo
```

### Ejercicio 6
**Enunciado:** Imprimir pares entre dos números.
```pseudocode
Algoritmo ParesEntre
    Definir a, b, i, inicio, fin como Entero
    Leer a, b
    Si a < b Entonces inicio <- a; fin <- b
    Sino inicio <- b; fin <- a
    FinSi
    Para i <- inicio Hasta fin Hacer
        Si i MOD 2 = 0 Entonces Escribir i
        FinSi
    FinPara
FinAlgoritmo
```

### Ejercicio 7
**Enunciado:** Tabla de multiplicar de un número.
```pseudocode
Algoritmo Tabla
    Definir num, i como Entero
    Leer num
    Para i <- 1 Hasta 10 Hacer
        Escribir num, " x ", i, " = ", num * i
    FinPara
FinAlgoritmo
```

### Ejercicio 8
**Enunciado:** Intervalo con validación, suma dentro, fuera y límites iguales.
```pseudocode
Algoritmo Intervalo
    Definir inf, sup, num, suma, fuera, iguales como Entero
    Repetir
        Leer inf, sup
        Si inf > sup Entonces Escribir "Error: inf <= sup"
        FinSi
    Hasta Que inf <= sup
    suma <- 0; fuera <- 0; iguales <- 0
    Repetir
        Leer num
        Si num = 0 Entonces Salir
        FinSi
        Si num > inf Y num < sup Entonces suma <- suma + num
        Sino Si num = inf O num = sup Entonces iguales <- iguales + 1
        Sino fuera <- fuera + 1
        FinSi
    Hasta Que num = 0
    Escribir "Suma dentro: ", suma, " | Fuera: ", fuera
    Si iguales > 0 Entonces Escribir "Hubo números iguales a los límites."
    FinSi
FinAlgoritmo
```

### Ejercicio 9
**Enunciado:** Potencia (base real, exponente entero) sin operador `^`.
```pseudocode
Algoritmo Potencia
    Definir base, exp, i, res como Real/Entero
    Leer base, exp
    res <- 1
    Para i <- 1 Hasta exp Hacer
        res <- res * base
    FinPara
    Escribir "Resultado: ", res
FinAlgoritmo
```

### Ejercicio 10
**Enunciado:** Tablas del 1 al 5.
```pseudocode
Algoritmo Tablas1a5
    Definir i, j como Entero
    Para i <- 1 Hasta 5 Hacer
        Para j <- 1 Hasta 10 Hacer
            Escribir i, " x ", j, " = ", i*j
        FinPara
    FinPara
FinAlgoritmo
```

### Ejercicio 11
**Enunciado:** Determinar si un número es primo.
```pseudocode
Algoritmo EsPrimo
    Definir num, i, divisores como Entero
    Leer num
    Si num <= 1 Entonces Escribir "No primo."
    Sino
        divisores <- 0
        Para i <- 2 Hasta RaizCuadrada(num) Hacer
            Si num MOD i = 0 Entonces divisores <- divisores + 1; Salir
            FinSi
        FinPara
        Si divisores = 0 Entonces Escribir "Primo."
        Sino Escribir "No primo."
        FinSi
    FinSi
FinAlgoritmo
```

### Ejercicio 12
**Enunciado:** Ahorro mensual variable durante un año.
```pseudocode
Algoritmo AhorroAnual
    Definir mes, deposito, total como Real
    total <- 0
    Para mes <- 1 Hasta 12 Hacer
        Leer deposito
        total <- total + deposito
        Escribir "Mes ", mes, " acumulado: ", total
    FinPara
FinAlgoritmo
```

### Ejercicio 13
**Enunciado:** Horas semanales (6 días) y sueldo de un empleado.
```pseudocode
Algoritmo SueldoEmpleado
    Definir dia, horas, precio, totalH, sueldo como Real
    Leer precio
    totalH <- 0
    Para dia <- 1 Hasta 6 Hacer
        Leer horas
        totalH <- totalH + horas
    FinPara
    sueldo <- totalH * precio
    Escribir "Horas: ", totalH, " | Sueldo: ", sueldo
FinAlgoritmo
```

### Ejercicio 14
**Enunciado:** Encuentro de coches en km 70 y 150 (mismo velocidad, opuestos).
```pseudocode
Algoritmo Encuentro
    Definir p1, p2, vel como Real
    p1 <- 70; p2 <- 150; vel <- 5 // velocidad unidad simulada
    Repetir
        p1 <- p1 + vel
        p2 <- p2 - vel
    Hasta Que p1 >= p2
    Escribir "Se encuentran cerca del km: ", p2
FinAlgoritmo
```

### Ejercicio 15
**Enunciado:** Pago progresivo (10, 20, 40...) por 20 meses.
```pseudocode
Algoritmo PagoProgresivo
    Definir mes, pago, total como Real
    pago <- 10; total <- 0
    Para mes <- 1 Hasta 20 Hacer
        total <- total + pago
        Escribir "Mes ", mes, ": ", pago
        pago <- pago * 2
    FinPara
    Escribir "Total: ", total
FinAlgoritmo
```

### Ejercicio 16
**Enunciado:** Sueldo semanal de N trabajadores y total empresa.
```pseudocode
Algoritmo NominaSimple
    Definir n, i, horas, precio, sueldo, totalE como Real
    Leer n, precio
    totalE <- 0
    Para i <- 1 Hasta n Hacer
        Leer horas
        sueldo <- horas * precio
        totalE <- totalE + sueldo
        Escribir "Trab ", i, ": ", sueldo
    FinPara
    Escribir "Total empresa: ", totalE
FinAlgoritmo
```

### Ejercicio 17
**Enunciado:** Horas por día de N trabajadores, sueldo y total.
```pseudocode
Algoritmo NominaDetallada
    Definir n, i, d, hDia, precio, sueldo, totalE como Real
    Leer n, precio
    totalE <- 0
    Para i <- 1 Hasta n Hacer
        sueldo <- 0
        Para d <- 1 Hasta 6 Hacer
            Leer hDia
            sueldo <- sueldo + hDia
        FinPara
        sueldo <- sueldo * precio
        totalE <- totalE + sueldo
        Escribir "Trab ", i, ": ", sueldo
    FinPara
    Escribir "Total empresa: ", totalE
FinAlgoritmo
```

### Ejercicio 18
**Enunciado:** Cronómetro (horas, minutos, segundos).
```pseudocode
Algoritmo Cronometro
    Definir h, m, s como Entero
    Para h <- 0 Hasta 23 Hacer
        Para m <- 0 Hasta 59 Hacer
            Para s <- 0 Hasta 59 Hacer
                Escribir h, ":", m, ":", s
                // Simular pausa de 1 segundo según lenguaje
            FinPara
        FinPara
    FinPara
FinAlgoritmo
```

### Ejercicio 19
**Enunciado:** Menú con opción Salir.
```pseudocode
Algoritmo Menu
    Definir op como Entero
    Repetir
        Escribir "1. Opción A\n2. Opción B\n3. Salir"
        Leer op
        Segun op Hacer
            1: Escribir "Ejecutando A..."
            2: Escribir "Ejecutando B..."
            3: Escribir "Saliendo..."
            De Otro Modo: Escribir "Inválida"
        FinSegun
    Hasta Que op = 3
FinAlgoritmo
```

### Ejercicio 20
**Enunciado:** Mostrar N primeros números primos.
```pseudocode
Algoritmo NPrimos
    Definir n, encontrados, cand, i, esP como Entero
    Leer n
    encontrados <- 0; cand <- 2
    Mientras encontrados < n Hacer
        esP <- Verdadero
        Para i <- 2 Hasta RaizCuadrada(cand) Hacer
            Si cand MOD i = 0 Entonces esP <- Falso; Salir
            FinSi
        FinPara
        Si esP Entonces Escribir cand; encontrados <- encontrados + 1
        FinSi
        cand <- cand + 1
    FinMientras
FinAlgoritmo
```

### Ejercicio 21
**Enunciado:** Sucesión de Fibonacci (N términos).
```pseudocode
Algoritmo Fibonacci
    Definir n, a, b, temp, i como Entero
    Leer n
    a <- 0; b <- 1
    Para i <- 1 Hasta n Hacer
        Escribir a
        temp <- a + b; a <- b; b <- temp
    FinPara
FinAlgoritmo
```

### Ejercicio 22
**Enunciado:** Suma de dígitos de un número.
```pseudocode
Algoritmo SumaDigitos
    Definir num, suma, dig como Entero
    Leer num
    suma <- 0
    Mientras num > 0 Hacer
        dig <- num MOD 10
        suma <- suma + dig
        num <- num DIV 10
    FinMientras
    Escribir "Suma: ", suma
FinAlgoritmo
```

### Ejercicio 23
**Enunciado:** Invertir número entero.
```pseudocode
Algoritmo Invertir
    Definir num, inv, dig como Entero
    Leer num
    inv <- 0
    Mientras num > 0 Hacer
        dig <- num MOD 10
        inv <- inv * 10 + dig
        num <- num DIV 10
    FinMientras
    Escribir "Invertido: ", inv
FinAlgoritmo
```

### Ejercicio 24
**Enunciado:** Verificar si es capicúa.
```pseudocode
Algoritmo Capicua
    Definir num, temp, inv, dig como Entero
    Leer num
    temp <- num; inv <- 0
    Mientras temp > 0 Hacer
        dig <- temp MOD 10; inv <- inv*10+dig; temp <- temp DIV 10
    FinMientras
    Si inv = num Entonces Escribir "Sí" Sino Escribir "No"
    FinSi
FinAlgoritmo
```

### Ejercicio 25
**Enunciado:** Listar divisores de un número.
```pseudocode
Algoritmo Divisores
    Definir num, i como Entero
    Leer num
    Para i <- 1 Hasta num Hacer
        Si num MOD i = 0 Entonces Escribir i
        FinSi
    FinPara
FinAlgoritmo
```

### Ejercicio 26
**Enunciado:** Verificar número perfecto.
```pseudocode
Algoritmo Perfecto
    Definir num, i, suma as Entero
    Leer num
    suma <- 0
    Para i <- 1 Hasta num DIV 2 Hacer
        Si num MOD i = 0 Entonces suma <- suma + i
        FinSi
    FinPara
    Si suma = num Entonces Escribir "Perfecto" Sino "No perfecto"
    FinSi
FinAlgoritmo
```

### Ejercicio 27
**Enunciado:** Triángulo rectángulo de asteriscos (creciente).
```pseudocode
Algoritmo TrianguloCreciente
    Definir n, i, j como Entero
    Leer n
    Para i <- 1 Hasta n Hacer
        Para j <- 1 Hasta i Hacer Escribir Sin Salto "*" FinPara
        Escribir ""
    FinPara
FinAlgoritmo
```

### Ejercicio 28
**Enunciado:** Pirámide centrada de asteriscos.
```pseudocode
Algoritmo Piramide
    Definir n, i, j, k como Entero
    Leer n
    Para i <- 1 Hasta n Hacer
        Para j <- 1 Hasta n-i Hacer Escribir Sin Salto " " FinPara
        Para k <- 1 Hasta 2*i-1 Hacer Escribir Sin Salto "*" FinPara
        Escribir ""
    FinPara
FinAlgoritmo
```

### Ejercicio 29
**Enunciado:** Triángulo invertido.
```pseudocode
Algoritmo TrianguloInv
    Definir n, i, j como Entero
    Leer n
    Para i <- n Hasta 1 Paso -1 Hacer
        Para j <- 1 Hasta i Hacer Escribir Sin Salto "*" FinPara
        Escribir ""
    FinPara
FinAlgoritmo
```

### Ejercicio 30
**Enunciado:** Rombo de asteriscos (altura impar).
```pseudocode
Algoritmo Rombo
    Definir n, i, j, k as Entero
    Leer n
    // Superior
    Para i <- 1 Hasta (n+1)/2 Hacer
        Para j <- 1 Hasta (n+1)/2-i Hacer Escribir Sin Salto " " FinPara
        Para k <- 1 Hasta 2*i-1 Hacer Escribir Sin Salto "*" FinPara
        Escribir ""
    FinPara
    // Inferior
    Para i <- (n-1)/2 Hasta 1 Paso -1 Hacer
        Para j <- 1 Hasta (n+1)/2-i Hacer Escribir Sin Salto " " FinPara
        Para k <- 1 Hasta 2*i-1 Hacer Escribir Sin Salto "*" FinPara
        Escribir ""
    FinPara
FinAlgoritmo
```

### Ejercicio 31
**Enunciado:** Tabla multiplicar 1-10 en cuadrícula.
```pseudocode
Algoritmo TablaCuadricula
    Definir i, j as Entero
    Para i <- 1 Hasta 10 Hacer
        Para j <- 1 Hasta 10 Hacer
            Escribir i*j, " "
        FinPara
        Escribir ""
    FinPara
FinAlgoritmo
```

### Ejercicio 32
**Enunciado:** Interés compuesto año a año.
```pseudocode
Algoritmo InteresCompuesto
    Definir cap, tasa, anios, i as Real/Entero
    Leer cap, tasa, anios
    Para i <- 1 Hasta anios Hacer
        cap <- cap * (1 + tasa/100)
        Escribir "Año ", i, ": ", cap
    FinPara
FinAlgoritmo
```

### Ejercicio 33
**Enunciado:** Cuenta bancaria (depósitos/retiros) hasta salir o saldo negativo.
```pseudocode
Algoritmo Cuenta
    Definir saldo, op, monto as Real
    saldo <- 0
    Repetir
        Leer op
        Si op = 1 Entonces Leer monto; saldo <- saldo + monto
        Sino Si op = 2 Entonces Leer monto
            Si monto > saldo Entonces Escribir "Insuficiente"
            Sino saldo <- saldo - monto
            FinSi
        FinSi
    Hasta Que op = 3 O saldo < 0
    Escribir "Final: ", saldo
FinAlgoritmo
```

### Ejercicio 34
**Enunciado:** Validador contraseña (≥8, mayús, número).
```pseudocode
Algoritmo ValidarPass
    Definir pass, len, i, tieneM, tieneN as Entero/Carácter/Booleano
    Repetir
        Leer pass
        len <- Longitud(pass); tieneM <- Falso; tieneN <- Falso
        Para i <- 1 Hasta len Hacer
            car <- Subcadena(pass,i,1)
            Si car >= 'A' Y car <= 'Z' Entonces tieneM <- Verdadero
            Sino Si car >= '0' Y car <= '9' Entonces tieneN <- Verdadero
            FinSi
        FinPara
    Hasta Que len >= 8 Y tieneM Y tieneN
    Escribir "Válida"
FinAlgoritmo
```

### Ejercicio 35
**Enunciado:** Contar dígito en secuencia terminada en -1.
```pseudocode
Algoritmo ContarDig
    Definir num, obj, dig, cont, temp as Entero
    Leer obj
    cont <- 0
    Repetir
        Leer num
        Si num = -1 Entonces Salir
        FinSi
        temp <- Abs(num)
        Mientras temp > 0 Hacer
            dig <- temp MOD 10
            Si dig = obj Entonces cont <- cont + 1
            FinSi
            temp <- temp DIV 10
        FinMientras
    Hasta Que Falso
    Escribir "Apariciones: ", cont
FinAlgoritmo
```

### Ejercicio 36
**Enunciado:** Mayor y menor de N números en una pasada.
```pseudocode
Algoritmo MayorMenor
    Definir n, i, num, mayor, menor as Entero
    Leer n
    Leer mayor; menor <- mayor
    Para i <- 2 Hasta n Hacer
        Leer num
        Si num > mayor Entonces mayor <- num
        Sino Si num < menor Entonces menor <- num
        FinSi
    FinPara
    Escribir "Mayor: ", mayor, " | Menor: ", menor
FinAlgoritmo
```

### Ejercicio 37
**Enunciado:** MCD con algoritmo de Euclides.
```pseudocode
Algoritmo MCD
    Definir a, b, temp as Entero
    Leer a, b
    Mientras b <> 0 Hacer
        temp <- b
        b <- a MOD b
        a <- temp
    FinMientras
    Escribir "MCD: ", a
FinAlgoritmo
```

### Ejercicio 38
**Enunciado:** MCM de dos números.
```pseudocode
Algoritmo MCM
    Definir a, b, mayor, mcm as Entero
    Leer a, b
    mayor <- a; Si b > a Entonces mayor <- b FinSi
    mcm <- mayor
    Mientras Verdadero Hacer
        Si mcm MOD a = 0 Y mcm MOD b = 0 Entonces Salir
        FinSi
        mcm <- mcm + mayor
    FinMientras
    Escribir "MCM: ", mcm
FinAlgoritmo
```

### Ejercicio 39
**Enunciado:** Lanzar dado hasta sacar 6.
```pseudocode
Algoritmo Dado6
    Definir lanz, intentos as Entero
    intentos <- 0
    Repetir
        lanz <- Aleatorio(1,6)
        intentos <- intentos + 1
    Hasta Que lanz = 6
    Escribir "Intentos: ", intentos
FinAlgoritmo
```

### Ejercicio 40
**Enunciado:** Decimal a binario.
```pseudocode
Algoritmo DecBin
    Definir num, res as Entero
    bin as Cadena
    Leer num
    bin <- ""
    Si num = 0 Entonces bin <- "0"
    Sino
        Mientras num > 0 Hacer
            res <- num MOD 2
            bin <- ConvertirATexto(res) + bin
            num <- num DIV 2
        FinMientras
    FinSi
    Escribir bin
FinAlgoritmo
```

### Ejercicio 41
**Enunciado:** Decimal a hexadecimal.
```pseudocode
Algoritmo DecHex
    Definir num, res as Entero
    hex as Cadena
    Leer num
    hex <- ""
    Si num = 0 Entonces hex <- "0"
    Sino
        Mientras num > 0 Hacer
            res <- num MOD 16
            Si res < 10 Entonces hex <- ConvertirATexto(res) + hex
            Sino hex <- Caracter(res-10+65) + hex
            FinSi
            num <- num DIV 16
        FinMientras
    FinSi
    Escribir hex
FinAlgoritmo
```

### Ejercicio 42
**Enunciado:** FizzBuzz hasta N.
```pseudocode
Algoritmo FizzBuzz
    Definir n, i as Entero
    Leer n
    Para i <- 1 Hasta n Hacer
        Si i MOD 15 = 0 Entonces Escribir "FizzBuzz"
        Sino Si i MOD 3 = 0 Entonces "Fizz"
        Sino Si i MOD 5 = 0 Entonces "Buzz"
        Sino i
        FinSi
    FinPara
FinAlgoritmo
```

### Ejercicio 43
**Enunciado:** Suma serie armónica.
```pseudocode
Algoritmo Armonica
    Definir n, i as Entero
    suma as Real
    Leer n
    suma <- 0
    Para i <- 1 Hasta n Hacer
        suma <- suma + 1.0/i
    FinPara
    Escribir suma
FinAlgoritmo
```

### Ejercicio 44
**Enunciado:** Suma de cuadrados 1 a N.
```pseudocode
Algoritmo SumaCuad
    Definir n, i, suma as Entero
    Leer n
    suma <- 0
    Para i <- 1 Hasta n Hacer
        suma <- suma + i*i
    FinPara
    Escribir suma
FinAlgoritmo
```

### Ejercicio 45
**Enunciado:** Bisiestos hasta año negativo.
```pseudocode
Algoritmo Bisiestos
    Definir anio as Entero
    Repetir
        Leer anio
        Si anio >= 0 Entonces
            Si (anio MOD 4=0 Y anio MOD 100<>0) O (anio MOD 400=0) Entonces "Bisiesto"
            Sino "No bisiesto"
            FinSi
        FinSi
    Hasta Que anio < 0
FinAlgoritmo
```

### Ejercicio 46
**Enunciado:** Semáforo (V 3s, A 1s, R 3s) N ciclos.
```pseudocode
Algoritmo Semaforo
    Definir ciclos, c, s as Entero
    Leer ciclos
    Para c <- 1 Hasta ciclos Hacer
        Escribir "VERDE (3s)"
        Para s <- 1 Hasta 3 Hacer FinPara
        Escribir "AMARILLO (1s)"
        Para s <- 1 Hasta 1 Hacer FinPara
        Escribir "ROJO (3s)"
        Para s <- 1 Hasta 3 Hacer FinPara
    FinPara
FinAlgoritmo
```

### Ejercicio 47
**Enunciado:** Generador contraseñas aleatorias longitud L, cantidad C.
```pseudocode
Algoritmo GenPass
    Definir cant, len, i, j, tipo as Entero
    pass as Cadena
    Leer cant, len
    Para i <- 1 Hasta cant Hacer
        pass <- ""
        Para j <- 1 Hasta len Hacer
            tipo <- Aleatorio(1,3)
            Si tipo = 1 Entonces pass <- pass + Caracter(Aleatorio(65,90))
            Sino Si tipo = 2 Entonces pass <- pass + Caracter(Aleatorio(97,122))
            Sino pass <- pass + ConvertirATexto(Aleatorio(0,9))
            FinSi
        FinPara
        Escribir "Pass ", i, ": ", pass
    FinPara
FinAlgoritmo
```

### Ejercicio 48
**Enunciado:** Contar vocales/consonantes hasta punto.
```pseudocode
Algoritmo VocCons
    Definir txt, i, v, c, ch as Entero/Carácter
    Leer txt
    v <- 0; c <- 0
    Para i <- 1 Hasta Longitud(txt) Hacer
        ch <- Subcadena(txt,i,1)
        Si ch = '.' Entonces Salir
        FinSi
        Si ch EN ['a','e','i','o','u','A','E','I','O','U'] Entonces v <- v+1
        Sino Si (ch >= 'A' Y ch <= 'Z') O (ch >= 'a' Y ch <= 'z') Entonces c <- c+1
        FinSi
    FinPara
    Escribir "V: ", v, " C: ", c
FinAlgoritmo
```

### Ejercicio 49
**Enunciado:** Progresión aritmética (inicio, diferencia, N términos).
```pseudocode
Algoritmo Progresion
    Definir n, a1, diff, i, val as Entero
    Leer a1, diff, n
    val <- a1
    Para i <- 1 Hasta n Hacer
        Escribir val
        val <- val + diff
    FinPara
FinAlgoritmo
```

### Ejercicio 50
**Enunciado:** Crecimiento poblacional con tasa %.
```pseudocode
Algoritmo Poblacion
    Definir pob, tasa, anios, i as Real/Entero
    Leer pob, tasa, anios
    Para i <- 1 Hasta anios Hacer
        pob <- pob * (1 + tasa/100)
        Escribir "Año ", i, ": ", Entero(pob)
    FinPara
FinAlgoritmo
```

### Ejercicio 51
**Enunciado:** Promedio notas M alumnos, N asignaturas.
```pseudocode
Algoritmo Notas
    Definir m, n, a, s, nota, sumA, sumT as Real
    Leer m, n
    sumT <- 0
    Para a <- 1 Hasta m Hacer
        sumA <- 0
        Para s <- 1 Hasta n Hacer
            Leer nota
            sumA <- sumA + nota
        FinPara
        Escribir "Prom alumno ", a, ": ", sumA/n
        sumT <- sumT + sumA
    FinPara
    Escribir "Prom general: ", sumT/(m*n)
FinAlgoritmo
```

### Ejercicio 52
**Enunciado:** Tabla multiplicar hasta límite.
```pseudocode
Algoritmo TablaLim
    Definir num, lim, i, res as Entero
    Leer num, lim
    Para i <- 1 Hasta 10 Hacer
        res <- num * i
        Si res <= lim Entonces Escribir res
        Sino Salir
        FinSi
    FinPara
FinAlgoritmo
```

### Ejercicio 53
**Enunciado:** Números Armstrong de 3 cifras.
```pseudocode
Algoritmo Armstrong
    Definir num, t, s, d as Entero
    Para num <- 100 Hasta 999 Hacer
        t <- num
        d <- t MOD 10; t <- t DIV 10
        s <- d^3 + (t MOD 10)^3 + (t DIV 10)^3
        Si s = num Entonces Escribir num
        FinSi
    FinPara
FinAlgoritmo
```

### Ejercicio 54
**Enunciado:** Cajero automático básico con menú.
```pseudocode
Algoritmo Cajero
    Definir saldo, op, monto as Real
    saldo <- 1000
    Repetir
        Leer op
        Segun op Hacer
            1: Escribir "Saldo: ", saldo
            2: Leer monto; saldo <- saldo + monto
            3: Leer monto
               Si monto > saldo Entonces "Insuficiente"
               Sino saldo <- saldo - monto
               FinSi
            4: "Saliendo"
            De Otro Modo: "Inválida"
        FinSegun
    Hasta Que op = 4
FinAlgoritmo
```

### Ejercicio 55
**Enunciado:** Factoriales de 1 a N.
```pseudocode
Algoritmo Factoriales
    Definir n, i, j, f as Entero
    Leer n
    Para i <- 1 Hasta n Hacer
        f <- 1
        Para j <- 1 Hasta i Hacer f <- f*j FinPara
        Escribir i, "! = ", f
    FinPara
FinAlgoritmo
```

### Ejercicio 56
**Enunciado:** Longitud máxima secuencia consecutiva positiva.
```pseudocode
Algoritmo SecPositiva
    Definir num, act, max as Entero
    act <- 0; max <- 0
    Repetir
        Leer num
        Si num > 0 Entonces
            act <- act + 1
            Si act > max Entonces max <- act
            FinSi
        Sino act <- 0
        FinSi
    Hasta Que num = 0
    Escribir "Máx consecutiva: ", max
FinAlgoritmo
```

### Ejercicio 57
**Enunciado:** Adivinar palabra letra por letra (10 intentos).
```pseudocode
Algoritmo Ahorcado
    Definir palabra, prog, letra, intentos, i, enc as Cadena/Entero/Booleano
    palabra <- "ALGORITMO"
    prog <- Repetir("_", Longitud(palabra))
    intentos <- 10
    Repetir
        Escribir prog, " | Intentos: ", intentos
        Leer letra
        enc <- Falso
        Para i <- 1 Hasta Longitud(palabra) Hacer
            Si Subcadena(palabra,i,1) = letra Entonces
                prog <- Subcadena(prog,1,i-1) + letra + Subcadena(prog,i+1)
                enc <- Verdadero
            FinSi
        FinPara
        Si No enc Entonces intentos <- intentos - 1
        FinSi
    Hasta Que prog = palabra O intentos = 0
    Si prog = palabra Entonces "Ganaste" Sino "Perdiste: ", palabra
    FinSi
FinAlgoritmo
```

### Ejercicio 58
**Enunciado:** Suma pares e impares entre 1 y N.
```pseudocode
Algoritmo SumaPI
    Definir n, i, sp, si as Entero
    Leer n
    sp <- 0; si <- 0
    Para i <- 1 Hasta n Hacer
        Si i MOD 2 = 0 Entonces sp <- sp + i
        Sino si <- si + i
        FinSi
    FinPara
    Escribir "Pares: ", sp, " | Impares: ", si
FinAlgoritmo
```

### Ejercicio 59
**Enunciado:** Calendario 7 columnas con desplazamiento inicial.
```pseudocode
Algoritmo Calendario
    Definir dias, desp, i, dia as Entero
    Leer dias, desp
    Para i <- 1 Hasta desp Hacer Escribir Sin Salto "   " FinPara
    dia <- 1
    Mientras dia <= dias Hacer
        Escribir Sin Salto dia, " "
        dia <- dia + 1
        Si (dia + desp - 1) MOD 7 = 0 Entonces Escribir ""
        FinSi
    FinMientras
FinAlgoritmo
```

### Ejercicio 60
**Enunciado:** Piedra, Papel o Tijera vs CPU con marcador.
```pseudocode
Algoritmo PPT
    Definir op, cpu, v, e, d as Entero
    v <- 0; e <- 0; d <- 0
    Repetir
        Leer op
        Si op >= 1 Y op <= 3 Entonces
            cpu <- Aleatorio(1,3)
            Si op = cpu Entonces e <- e + 1; "Empate"
            Sino Si (op=1 Y cpu=3) O (op=2 Y cpu=1) O (op=3 Y cpu=2) Entonces v <- v + 1; "Ganaste"
            Sino d <- d + 1; "Perdiste"
            FinSi
        Sino Si op = 4 Entonces "Salir"
        Sino "Inválida"
        FinSi
    Hasta Que op = 4
    Escribir "V:", v, " E:", e, " D:", d
FinAlgoritmo
```

---
💡 **Nota pedagógica:** Este pseudocódigo está diseñado para ser **independiente del lenguaje**. Para implementarlo en Python, Java, C++, JS o cualquier otro, solo necesitas mapear:
- `Leer` → `input()`, `cin`, `Console.ReadLine()`, `prompt()`
- `Escribir` → `print()`, `cout`, `Console.Write()`, `alert()`
- `Aleatorio(a,b)` → `random.randint(a,b)`, `rand() % (b-a+1) + a`, etc.
- `RaizCuadrada(x)` → `sqrt(x)`, `Math.sqrt(x)`

¿Deseas que te entregue **las soluciones completas en un lenguaje específico** (Python, Java, C++, JavaScript, etc.) o que profundice en la lógica de algún ejercicio en particular?
