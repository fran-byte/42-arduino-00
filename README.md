# 42-arduino-00

# ex00 

✅ Proyecto 1: Semáforo Básico con Botón (Tinkercad)

Nivel: principiante
Formato: sin clases, lógica en loop() y funciones

💡 Idea:

Simular un cruce peatonal. El sistema se mantiene en verde para coches, pero si alguien pulsa el botón, después de un ciclo se cambia a rojo y deja pasar a los peatones.

🧩 Componentes:

3 LEDs (rojo, amarillo, verde)

1 botón (con resistencia pull-down o usando INPUT_PULLUP)

Arduino Uno, o variantes. 


🛠️ Funcionalidad:

Estado por defecto: luz verde.

Al pulsar el botón: espera 2 segundos, cambia a amarillo por 1 segundo, luego a rojo por 5 segundos, y luego vuelve a verde.

El botón se ignora si ya está en proceso de cambio.


🧠 Enfoque educativo:

Uso de digitalRead, digitalWrite, delay.

Estado controlado por variables (estado, espera).

Práctica de estructuras condicionales (if) y lógica secuencial.



---

✅ Proyecto 2: Termómetro con Alarma y Umbral Ajustable (Tinkercad)

Nivel: principiante–intermedio
Formato: sin clases, funciones separadas

💡 Idea:

Leer temperatura de un sensor (simulado) y activar una alarma (LED/buzzer) si supera cierto valor.

🧩 Componentes:

Sensor TMP36 o LM35 (simulado)

LED rojo (alarma)

Potenciómetro (para ajustar el umbral)

Arduino Uno


🛠️ Funcionalidad:

Leer temperatura del sensor analógico.

Leer el umbral desde el potenciómetro.

Si la temperatura supera el umbral, se activa el LED.

Mostrar datos en consola serial (Serial.print).


🧠 Enfoque educativo:

Introducción a sensores analógicos (analogRead)

Conversión de valores (de ADC a °C)

Comparaciones, uso de map() para ajustar escala

Estructura del programa clara y segmentada en funciones: leerTemperatura(), leerUmbral(), activarAlarma().



---

✅ Proyecto 3: Detector de Luz Dual (con hardware real en Protoboard o simulador avanzado)

Nivel: intermedio
Formato: funciones + lógica más compleja

💡 Idea:

Un sistema con dos sensores de luz (LDRs) que "decide" hacia dónde girar o encender LEDs, según cuál detecta más luz.

🧩 Componentes:

2 LDRs con resistencias (divisor de voltaje)

2 LEDs (simulan motores, por ejemplo)

Arduino Uno, o similar. 


🛠️ Funcionalidad:

Se comparan las dos lecturas analógicas.

Si hay más luz en la izquierda, se enciende el LED izquierdo (o simula movimiento).

Si hay más en la derecha, se activa el otro.

Si es parejo, ambos apagados (o ambos encendidos).


🧠 Enfoque educativo:

Introducción al comportamiento reactivo.

Comparación de sensores.

Uso de funciones simples como compararLuz() o decidirMovimiento().

Se puede escalar fácilmente (se puede conectar a servos o motores reales más adelante).



---
