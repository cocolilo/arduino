Código que simula puertas lógicas con una placa Node MCU V3 conectada a un potenciómetro, dos pulsadores en configuración
PULL DOWN y un led RGB de ánodo común. Las lecturas del potenciometro están escaladas de 0 a 100.

Se seleccionan las puertas lógicas con el potenciómetro, el intervalo de lectura del potenciómetro está dividido de la
siguiente forma: 

   *  [0-20]: compuerta AND
   *  ]20-40]: compuerta OR
   *  ]40-60]: compuerta NAND
   *  ]60-80]: compuerta NOR
   *  ]80-100]: compuerta XOR
   
Las entradas de la puerta lógica son los dos pulsadores, y se enciende el led RGB solo si la puerta lógica da valor 1,
además el led se enciende con un color determinado dependiendo de la puerta lógica seleccionada 

Conclusión: Es posible simular puertas lógicas usando software, aunque las que están implementadas en este código son las básicas estoy seguro de que se podrían añadir muchas más. Algo que quisiera mencionar es que la función implementada que imprime por el puerto serial la información sobre las entradas y salidas ocupa muchos recursos de la placa, y se pone leeenta a veces... Al parecer no fue lo más eficiente
