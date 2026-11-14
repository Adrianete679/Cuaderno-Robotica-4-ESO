# Prácticas

## Práctica 1 - Encendido alternativo de diodos leds
<img width="750" height="400" alt="Práctica 1" src="https://github.com/user-attachments/assets/99b01575-6798-4a6f-8c75-387cbbe79724" />

[![](https://img.youtube.com/vi/2f6OHwZokGQ/0.jpg)](https://www.youtube.com/watch?v=2f6OHwZokGQ)


### ¿En qué consiste?:
Consiste en encender y apagar dos LED alternativamente. Cuando uno está encendido, el otro está apagado. Cada segundo cambian de estado.

### Código explicado:
-void setup(): ejecuta las instrucciones una sola vez cuando se inicia Arduino.

-pinMode(13, OUTPUT): indica que el pin 13 va a enviar electricidad para controlar un LED.

-pinMode(7, OUTPUT): hace lo mismo con el pin 7.

-void loop(): hace que las instrucciones se repitan continuamente.

-digitalWrite(13, LOW): apaga el LED conectado al pin 13.

-digitalWrite(7, HIGH): enciende el LED conectado al pin 7.

-delay(1000): espera un segundo.

## Práctica 2 - Pulsador
<img width="750" height="400" alt="image" src="https://github.com/user-attachments/assets/20544824-5b60-4e81-85fe-0a64e270d636" />

[![](https://img.youtube.com/vi/-WE_l8MV6Dg/0.jpg)](https://www.youtube.com/watch?v=-WE_l8MV6Dg)


### ¿En qué consiste?:
Consiste en utilizar un pulsador para encender y apagar un LED. Cuando pulsamos el botón, se enciende el LED y cuando lo soltamos, se apaga. Además, Arduino muestra en el ordenador si el botón está pulsado o no.

### Código explicado:
-#define pin2 2: crea un nombre para identificar el pin 2, donde está conectado el pulsador.

-#define pin13 13: crea un nombre para identificar el pin 13, donde está conectado el LED.

-int valor2: crea una variable para guardar si el pulsador está pulsado o no.

-pinMode(pin2, INPUT): indica que el pin 2 va a recibir información del pulsador.

-Serial.begin(9600): permite que Arduino se comunique con el ordenador.

-digitalRead(pin2): comprueba si el pulsador está pulsado o no.

-if: sirve para comprobar si se cumple una condición.

-valor2 == HIGH: comprueba si el valor recibido es HIGH.

-digitalWrite(pin13, LOW): apaga el LED.

-Serial.println("No Pulsado"): muestra el mensaje «No Pulsado» en el ordenador.

-valor2 == LOW: comprueba si el valor recibido es LOW.

-digitalWrite(pin13, HIGH): enciende el LED.

-Serial.println("Pulsado"): muestra el mensaje «Pulsado».

## Práctica 3 - Potenciómetro. Mapear
<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e271ff45-8924-4f87-9f34-69d523f1de85" />
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/b0ff7c84-e040-406f-8333-7ff8874869f9" />

[![](https://img.youtube.com/vi/u_LzLcUyPQk/0.jpg)](https://www.youtube.com/watch?v=u_LzLcUyPQk)
(Vídeo hecho por mi compañero Lorenzo Manuel Latorre Martínez)

### ¿En qué consiste?:
Consiste en utilizar un potenciómetro para cambiar un valor girándolo. Arduino lee ese valor y lo muestra en el ordenador. Cuanto más giramos el potenciómetro, más cambia el número que aparece.

### Código explicado:
-int P2 = A2: indica que el potenciómetro está conectado a la entrada A2 de Arduino.

-float valorpotenciometro = 0: crea una variable para guardar el valor del potenciómetro. Puede guardar números con decimales.

-analogRead(P2): lee el valor que está enviando el potenciómetro. En Arduino Uno puede ir de 0 a 1023.

-Serial.println(valorpotenciometro): muestra el valor en el ordenador.

-delay(500): espera medio segundo antes de volver a leer el potenciómetro.

## Práctica 4 - Mapeado de datos del potenciómetro
<img width="600" height="250" alt="image" src="https://github.com/user-attachments/assets/e271ff45-8924-4f87-9f34-69d523f1de85" /> 

(Es la misma foto que la de la práctica anterior porque es el mismo montaje)
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/d6bdf9bb-7462-4cc4-8a5b-28144c832913" />

[![](https://img.youtube.com/vi/FqHJXZcOIXY/0.jpg)](https://www.youtube.com/watch?v=FqHJXZcOIXY)
(Vídeo hecho por mi compañero Lorenzo Manuel Latorre Martínez)

### ¿En qué consiste?:
Consiste en cambiar los valores que obtenemos del potenciómetro. En vez de trabajar con números de 0 a 1023, los transformamos para que vayan de 0 a 100. Así resulta más fácil entenderlos.

### Código explicado:
-int resultado = 0: crea una variable para guardar el nuevo valor.

-map(valorpotenciometro, 0, 1023, 0, 100): cambia el valor del potenciómetro de una escala de 0-1023 a otra de 0-100.

-Serial.println(resultado): muestra el nuevo valor en el ordenador.

## Práctica 5 - PWM
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/0b2ccd75-7da8-470e-973b-5b857f0ee50d" />
<img width="600" height="350" alt="image" src="https://github.com/user-attachments/assets/12b242d2-30b4-4000-b5ca-c77bb485173f" />

[![](https://img.youtube.com/vi/ZORLppsyEgE/0.jpg)](https://www.youtube.com/watch?v=ZORLppsyEgE)
(Vídeo hecho por mi compañero Lorenzo Manuel Latorre Martínez)

### ¿En qué consiste?:
Consiste en controlar el brillo de un LED utilizando un potenciómetro. Al girar el potenciómetro, podemos hacer que el LED brille más o menos.

### Código explicado:
-int LED1 = 11: indica que el LED está conectado al pin 11.

-int DutyCycle: crea una variable para guardar la intensidad que tendrá el LED.

-map(valorpotenciometro, 0, 1023, 0, 255): transforma los valores del potenciómetro a una escala de 0 a 255.

-analogWrite(LED1, DutyCycle): controla el brillo del LED según el valor que tenga la variable DutyCycle.

## Práctica 6 - Ultrasonido
<img width="600" height="250" alt="Imgen de Cerca" src="https://github.com/user-attachments/assets/fa4761f3-ff90-4520-ae9f-ee7bdf58f830" />
<img width="650" height="300" alt="Codigo 1ºParte" src="https://github.com/user-attachments/assets/dd13b153-efe6-4ea8-a9cc-337847d39a53" />
<img width="650" height="300" alt="Codigo 2ºParte" src="https://github.com/user-attachments/assets/2bfe9100-4cc3-43e6-bf75-a1ff9217a781" />

[![](https://img.youtube.com/vi/EXzA4VjIh4Y/0.jpg)](https://www.youtube.com/watch?v=EXzA4VjIh4Y)
(Vídeo hecho por mi compañero Lorenzo Manuel Latorre Martínez)

### ¿En qué consiste?:
Consiste en utilizar un sensor ultrasónico para saber a qué distancia está un objeto. Si el objeto está a menos de 15 centímetros, se enciende un LED. Si está a 15 centímetros o más, el LED se apaga.

### Código explicado:
-#include <Ultrasonic.h>: añade una biblioteca que permite utilizar el sensor ultrasónico.

-int ECHO_PIN = 13: indica que el cable ECHO del sensor está conectado al pin 13.

-int TRIG_PIN = 12: indica que el cable TRIG está conectado al pin 12.

-int LED1 = 8: indica que el LED está conectado al pin 8.

-Ultrasonic Chorifletes(TRIG_PIN, ECHO_PIN): crea un objeto llamado Chorifletes para poder utilizar el sensor.

-Serial.println("Aviso a 15 cm"): muestra el mensaje «Aviso a 15 cm» en el ordenador.

-Serial.print(Chorifletes.Ranging(CM)): mide la distancia a la que está el objeto y muestra el resultado.

-Serial.println(" cm"): escribe la unidad de medida, centímetros.

-if (Chorifletes.Ranging(CM) < 15): comprueba si el objeto está a menos de 15 centímetros.

-digitalWrite(LED1, HIGH): enciende el LED si el objeto está a menos de 15 centímetros.

-else: indica lo que tiene que hacer Arduino si no se cumple la condición anterior.

-digitalWrite(LED1, LOW): apaga el LED si el objeto está a 15 centímetros o más.

## Práctica 7 - Servomotor
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Aquí estaría la práctica explicada

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

# Retos

## Reto 1
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Consiste en montar un circuito con 5 LED y un potenciómetro para controlar la luz de los LED. Cuando el potenciómetro esté al mínimo, todos los LED estarán apagados. Al girarlo, el primer LED empezará a iluminarse poco a poco hasta llegar a su máxima luminosidad, después empezará a encenderse el segundo y hará lo mismo, y esto se hará con los cinco LED.

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

## Reto 2
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Consiste en utilizar un sensor ultrasónico y dos LED para crear una especie de sistema de emergencia. Cuando un objeto se acerque al sensor, los dos LED irán aumentando su brillo. Cuanto más cerca esté el objeto, más luz tendrán los LED.

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

## Reto 3
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Consiste en modificar la práctica del ultrasonido añadiendo un potenciómetro. Este servirá para elegir la distancia a la que queremos que se encienda el LED de emergencia.

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

## Reto 4 
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Consiste en utilizar un potenciómetro para controlar el movimiento de un servomotor. Al girar el potenciómetro, el servomotor cambiará su posición según el valor que le indiquemos.

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

## Reto 5
Aquí iría la imagen del montaje y del código, y el vídeo, pero no me ha dado tiempo a hacerlo.

### ¿En qué consiste?:
Consiste en utilizar un sensor ultrasónico para controlar un servomotor según la distancia a la que esté un objeto. El sensor medirá la distancia y, dependiendo de lo cerca o lejos que esté el objeto, el servomotor se moverá a una posición determinada.

### Código explicado:
Aquí estaría el código explicado pero no me ha dado tiempo a hacerlo

