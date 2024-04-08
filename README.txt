Esse projeto foi criado com a intenção de ser implementado em lugares onde são armazenados vinhos, pois eles precisam ser pouco iluminados para os vinhos continuarem em boa qualidade. O sistema captura a luz ambiente com um LDR (Light Dependent Resistor) e, baseado no nível de luz, um LED é aceso. O verde para caso a iluminação seja ideal, o amarelo para caso seja ideal, e o vermelho para caso a iluminação esteja em situação de perigo para os vinhos. Caso isso ocorra, um piezo é acionado, tocando um alarme por 3 segundos. Caso a situação de alerta continue, o piezo é reacionado depois de 10 segundos desde o fim do último alarme.

Foram usados no projeto:
- Arduino UNO R3
- Protoboard.
- 3 LEDs, um vermelho, um amarelo e um verde.
- Um buzzer (piezo).
- Um LDR.
- 3 resistores de 220 Ohms.
- 1 resistor de 10 kOhms.
- 14 cabos jumpers (macho-macho).
- Arduino IDE (para a compilação e upload do código).

Para reproduzir o projeto, é preciso ligar os resistores de 220 Ohms em série com os LEDs, e os conectar nos pins digitais do Arduino. Ligando a outra perna dos LEDs à terra (GND). O piezo deve ser ligado a outro pin digital do Arduino, e ligado à terra em sua outra perna. Já o LDR, o fotoresistor, tem que ser ligado em série com um resistor de 10 kOhms, ligado à terra em sua outra perna, e, na primeira perna, tem que ser conectado a um dos pins Analog In do Arduino. Por fim, é preciso conectar os pins GND e 5V do Arduino na sua respectiva entrada no protoboard, e o conectar em um compilador, em qualquer dispositivo que possua um. Caso os LED vermelho, amarelo e verde estejam nos pins 13, 12, 11, o piezo no pin 9, e o LDR no pin A0, o código já imbutido no projeto do GitHub funcionará automaticamente.
