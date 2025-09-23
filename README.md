# Controlador-MIDI---Raspberry-Pi-Pico
Repositorio del proyecto, controlador MIDI 

Este proyecto surgio como respuesta a un problema que tenia. Soy guitarrista de habitacion, normalmente toco canciones con mi guitarra conectada a la PC donde es procesada por diferentes pedales de efectos, amplificadores, cajas o gabinetes, etc (mayormente los conocidos Neural DSP). El tema es cuando una cancion necesita cambiar rapidamente de, vamos a llamarlos, Presets, estos cambios se pueden automatizar pero la idea es poder tocar en tiempo real como si fuera en vivo.

Entonces, todo esto seria posible con un controlador MIDI que envie "señales" y la PC, a travez de un Script, las interprete, traduzca a mensajes MIDI y los envie al DAW (en mi caso Reaper, pero deberia funcionar con cualquier otro).

Por lo tanto, de ahi surgio mi investigacion, por una cuestion de aprendizaje y de entretenimiento, opté por crear un controlador propio, totalmente customizable, a conseguir uno standard del mercado.



Temas 
  - [Por que Raspberry Pi Pico?](#por-que-raspberry-pi-pico)
  - [Tipos de Switches](#tipos-de-switches)
  - [Potenciometros VS Encoders](#potenciometros-vs-encoders) 



---

## Por que Raspberry Pi Pico?

---

## Tipos de Switches
En un microcontrolador como la Raspberry Pi Pico se pueden usar una gran cantidad de tipos de botones.
Hay momentaneos, fijos(al soltarlos quedan activos), switches de llave, y muchos mas.

En este proyecto lo ideal es switches momentaneos, ya que al "pisarlo", se lee la señal y no es necesario que quede fijo ya que eso lo interpreta el plugin mismo.


Switch SPST momentaneo de 2 pines. (El que vamos a usar).

<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/17e246d7-9da3-4dea-b4a8-b0e387b4df0a" />

Otros Switches:

Switch 3PDT, fijo, usado generalmente en pedales "reales".

<img width="100" height="100" alt="Image" src="https://github.com/user-attachments/assets/4f1f8a2b-f182-4a67-8a08-1b82e0777838" />
---

## Potenciometros VS Encoders
