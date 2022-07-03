# ESP32-CNC-SHIELD

Este proyecto como un proyecto privado para poder usar el modulo devkit ESP32 con GRBL para mis máquinas CNC actuales, para sustituir los actuales Arduino Uno con Prontoneers CNC SHIELD(ambos originales) con GRBL V1.1. 
Así poder ejecutar el código CNC desde la tarjeta SD atravéz de la interfaz web sin necesidad de tener el ordenador conectado.
El mi máquina grande (385x325x95) tengo finales de carrera (X, Y, Z), probe, nebulizador y relé para el fresador. 
Uso motores Nema23 de 2,8A y drivers DRV8825 en medio micro paso en todos los ejes para poder usar la máxima fuerza, ya que corto bastante aluminio, aparte de: madera, plástico y pcb:s. Esto es justo lo que busco, no necesito más caracteristicas.
Bart Dring ha hecho un trabajo estupendo con el port y adaptaciones para nueva funciones, pero yo no las necesito en estas máquinas.
Por eso he quitado todo menos lo antes mencionado, inclusive los pines para jumpers para configurar los pasos(MS0,MS1 y MS2).
Si uno quiere se puede facilmente puentear el MS0 con MS1 y MS2 así llega los 3,3v y obtiene 256 micropasos.

La versión V1.0 fue muy instructivo, pero había hecho las pistas más estrechas a 0,5mm pero no fue suficiente, la fresa los comió en algunos sitios. Así que decidí hacer una nueva versión, además el tamaño no era tan bueno para poder fresar dos en la misma placa pcb(150x100).

La versión V1.1 tiene un par de cambios de tamaño y emplazamiento de componentes, para poder fresar 2 unidades en una placa pcb de 150x100mm.
Ahora mide 66x72. Lo he hecho tan grande porque la placa pcb que uso es de un lado solo y necesito espacio para las pistas. 
Sí funciona seguramente haré una version SMD con conectores JST para los cables.
