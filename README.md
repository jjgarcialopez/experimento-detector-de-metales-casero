# experimento-detector-de-metales-casero
Nota:  todas las instrucciones y el codigo se encuentran en el documento word que esta adjunto en este repositorio, debe descargarlo para poder visualizar el contenido. 
haga click donde esta el titulo Configuracion para leer señales pwm y luego de click en donde dice View Raw, y se descargara el documento con la información.


Configuración para leer las señales PWM con arduino.

// Declarar una variable para almacenar el valor leído
int valorAnalogico = 0;

void setup() {
  // Inicializar el puerto serie a una velocidad de 9600 baudios
  Serial.begin(9600);
}

void loop() {
  // Leer el valor analógico del pin A0
  valorAnalogico = analogRead(A0);

  // Imprimir el valor leído en el monitor serial
  Serial.println(valorAnalogico);

  // Esperar un breve tiempo antes de leer el siguiente valor
  delay(100);
}
