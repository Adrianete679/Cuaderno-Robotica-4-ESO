# Prácticas

## Práctica 1 - Encendido alternativo de diodos leds
<img width="750" height="400" alt="image" src="https://github.com/user-attachments/assets/1e4e6b92-9365-46fa-ba3a-29d16101efa0" />

Esta práctica consiste en hacer un encendido alternativo de dos diodos LEDS, el primer LED en encenderse es el rojo y el segundo el azul. 
El código está compuesto por:
- void setup: sirve para ejecutar un bloque de código una sola vez justo cuando la placa se enciende o se reinicia.
- pinMode(OUTPUT): configura un pin digital específico como salida, para que pueda enviar energía o señales eléctricas a un componente.
- void loop: sirve para ejecutar un bloque de código de forma continua e infinita.
- digitalWrite(LOW): sirve para decir que un pin digital está apagado 
- digitalWrite(HIGH): sirve para decir que un pin digital está encendido.
- delay(1000): se utiliza para indicar que entre una acción y la otra debe haber un tiempo de espera, en este caso de 1 segundo. Este tiempo se indica en milisegundos.
## Práctica 2 - Pulsador
<img width="750" height="400" alt="image" src="https://github.com/user-attachments/assets/20544824-5b60-4e81-85fe-0a64e270d636" />

Esta práctica cosiste en hacer que un diodo LED que está encendido se apague utilizando un pulsador. 
El código está compuesto por:
- #define:
- int valor: 
- pinMode(INPUT): sirve para configurar un pin específico como entrada digital.
- Serial.begin():
- valor:
- digitalRead
- digitalWriteç
- serial.println
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
