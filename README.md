# Prácticas

## Práctica 1 - Encendido alternativo de diodos leds
<img width="750" height="400" alt="image" src="https://github.com/user-attachments/assets/1e4e6b92-9365-46fa-ba3a-29d16101efa0" />

¿En qué consiste?
Consiste en encender y apagar dos LED de forma alternativa. Cuando uno está encendido, el otro está apagado. Cada segundo cambian de estado.

Código explicado:
- void setup(): ejecuta las instrucciones una sola vez al iniciar Arduino.
- pinMode(13, OUTPUT): configura el pin 13 como salida.
- pinMode(7, OUTPUT): configura el pin 7 como salida.
- void loop(): repite las instrucciones continuamente.
- digitalWrite(13, LOW): apaga el LED del pin 13.
- digitalWrite(7, HIGH): enciende el LED del pin 7.
- delay(1000): espera un segundo.
## Práctica 2 - Pulsador
<img width="750" height="400" alt="image" src="https://github.com/user-attachments/assets/20544824-5b60-4e81-85fe-0a64e270d636" />

¿En qué consiste?
Consiste en utilizar un pulsador para controlar un LED. Cuando pulsamos el botón, el LED se enciende; cuando lo soltamos, se apaga. También muestra en el monitor serie si está pulsado o no.

Código explicado:
-#define pin2 2: asigna el nombre pin2 al pin 2.
-#define pin13 13: asigna el nombre pin13 al pin 13.
-int valor2: crea una variable para guardar el estado del pulsador.
-INPUT: configura el pin como entrada.
-Serial.begin(9600): inicia la comunicación con el ordenador.
-digitalRead(pin2): lee el estado del pulsador.
-if: comprueba si se cumple una condición.
-valor2 == HIGH: comprueba si el pulsador está sin pulsar o no.
-digitalWrite(pin13, LOW): apaga el LED.
-Serial.println("No Pulsado"): indica que no está pulsado.
-valor2 == LOW: comprueba si el pulsador está pulsado o no.
-digitalWrite(pin13, HIGH): enciende el LED.
-Serial.println("Pulsado"): indica que está pulsado.
## Práctica 3 - Potenciómetro. Mapear
<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e271ff45-8924-4f87-9f34-69d523f1de85" />
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/b0ff7c84-e040-406f-8333-7ff8874869f9" />

Esta práctica consiste en obtener distintos valores, del 0 al 1023, utilizando el mapeado.
El código está compuesto por:
- Escribir
- 
## Práctica 4 - Mapeado de datos del potenciómetro
<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e271ff45-8924-4f87-9f34-69d523f1de85" /> 

(Es la misma foto que la de la práctica anterior porque es el mismo montaje)
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/d6bdf9bb-7462-4cc4-8a5b-28144c832913" />

Esta práctica consiste en hacer que los valores de un potenciómetro, que va de 0 hasta 1224, se convieran en otros valores, en este caso los he convertido en valores de 0 a 100.
El código está compuesto por:
- mapear: sirve para hacer equivalentes los valores de dos objetos/elementos. Osea, que el valor máximo de un elemento sea el valor máximo de otro elemento que su máximo se mas elevado.
-
## Práctica 5 - PWM
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/0b2ccd75-7da8-470e-973b-5b857f0ee50d" />
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/12b242d2-30b4-4000-b5ca-c77bb485173f" />

Esta práctica consiste en hacer que la intensidad de un diodo led vaya aumentando o disminuyendo, dependiendo que que tanto gires el pntenciometro. Cuanto más gires el potenciometro, más aumentará o disminuirá la intensidad luminosa. 
El código está compuesto por:
- Escribir
-
## Práctica 6 - Ultrasonido
<img width="600" height="250" alt="Imgen de Cerca" src="https://github.com/user-attachments/assets/fa4761f3-ff90-4520-ae9f-ee7bdf58f830" />
<img width="650" height="300" alt="Codigo 1ºParte" src="https://github.com/user-attachments/assets/dd13b153-efe6-4ea8-a9cc-337847d39a53" />
<img width="650" height="300" alt="Codigo 2ºParte" src="https://github.com/user-attachments/assets/2bfe9100-4cc3-43e6-bf75-a1ff9217a781" />

Esta práctica consiste en 
El código está compuesto por:
- Escribir
- 
## Práctica 7 - Servomotor


Esta práctica consiste en 
El código está compuesto por:
- Escribir
- 

# Retos

## Reto 1


Este reto trata sobre un control de ledes con un potenciómetro. Diseñar, montar y programar un sistema que permita controlar 5 diodos LED (protegidos con una única resistencia) mediante un potenciómetro. El funcionamiento debe ser el siguiente: con el potenciómetro en valor mínimo, todos los ledes estarán apagados. Conforme subamos el valor del potenciómetro, el diodo 1 (solo este) debe ir incrementando su valor de luminosidad. Cuando el diodo 1 esté completamente iluminado, el 2 empezará a encenderse con una iluminación creciente hasta que llegue a su tope. Eso mismo deberemos hacer con todos los diodos 1, 2, 3, 4 y 5. Para ello os recomiendo utilizar unos condicionales, establecer valores frontera y mezclar lo aprendido en las prácticas anterores.
El código a sido explicado en prácticas anteriores
## Reto 2


Este reto consiste en
El código a sido explicado en prácticas anteriores
## Reto 3


Este reto consiste en
El código a sido explicado en prácticas anteriores
## Reto 4 


Este reto consiste en
El código a sido explicado en prácticas anteriores
