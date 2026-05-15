# estacionMeteorologica
  El objetivo fue diseñar una estación meteorológica que mida variables ambientales, almacene y visualice dichos datos localmente y en la nube. Por último el sistema debe ser “offline resilience”.

Específicamente, el sistema deberá tener las siguientes características:

  * Medir temperatura, humedad y presión. 
  * Visualizar las variables en la web, tanto local como cloud. Si es en un gráfico en función del tiempo, mejor. 
      ○ Localmente: Red LAN. 
      ○ Cloud: Cualquier servicio gratuito disponible para almacenar datos de IoT.

  Este proyecto consistió en la implementación de un sistema embebido, utilizando el microcontrolador ESP8266, que mediante sus dos sensores BMP280 y DHT11, lograba obtener datos de la temperatura, humedad y presión. Se utilizó también un servicio en la nube (ThingSpeak) donde se envían los datos para almacenarlos allí. Para lograr la comunicación entre los sensores y la placa, se utilizó un protocolo en específico el cual es el I2C.
