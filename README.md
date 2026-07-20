# DD Trainer — Simulador interactivo DD-602 / DD-1000

[![Versión](https://img.shields.io/badge/versión-1.4-5ce1dc?style=flat-square)](#versión-14)
[![Uso](https://img.shields.io/badge/uso-educativo-f4b64a?style=flat-square)](#aviso)
[![Sin instalación](https://img.shields.io/badge/instalación-no_requerida-7fd1cc?style=flat-square)](#cómo-usarlo)

Simulador educativo e interactivo del módulo de batería electrónica **DD-602 / DD-1000**, creado para aprender a utilizar sus controles desde una PC.

Reproduce visualmente el panel frontal y trasero, permite utilizar sus botones, rueda DATA, pads, metrónomo, grabación y ajustes de cada instrumento. También incluye un recorrido guiado que comprueba las acciones realizadas por el usuario.

## Características

- Interfaz inspirada en el módulo DD-602 / DD-1000.
- Vista frontal, vista 3D y representación del panel trasero.
- Rueda **DATA** interactiva y giratoria.
- Botones **PAGE**, **SELECT**, **SAVE / ENTER**, **TEMPO / TAP** y **RECORD** funcionales.
- Control de volumen general, entrada AUX y acompañamiento.
- Volumen y paneo independientes para cada instrumento y cada kit.
- Ajustes de sensibilidad, ganancia y curva de velocidad.
- Metrónomo con tempo regulable.
- Grabación y reproducción de una interpretación.
- Pads virtuales controlables con mouse o teclado.
- Ocho prácticas guiadas con progreso reiniciable.
- Funcionamiento local sin conexión a Internet.

## Cómo usarlo

1. Descarga o clona este repositorio.
2. Conserva `index.html`, `app.js` y `app.css` en la misma carpeta.
3. Abre `index.html` con Chrome, Edge, Firefox o Brave.
4. Pulsa **POWER**.
5. Sube poco a poco **MAIN VOLUME**.
6. Usa los pads virtuales o las teclas indicadas abajo.

No necesita instalación, servidor ni conexión a Internet.

## Controles del teclado

| Tecla | Instrumento |
|---|---|
| `A` | Snare |
| `S` | Hi-Hat |
| `D` | Tom 1 |
| `F` | Tom 2 |
| `G` | Tom 3 |
| `H` | Ride |
| `J` | Crash |
| `Espacio` | Kick |

## Controles principales

### Rueda DATA

La rueda DATA modifica el parámetro seleccionado en la pantalla. Puedes controlarla de cuatro formas:

- Arrastrándola horizontalmente con el mouse.
- Girando la rueda del mouse sobre ella.
- Pulsando el lado `−` o `+`.
- Usando las flechas del teclado cuando tiene el foco.

### PAGE − / +

Permite avanzar o retroceder por las páginas disponibles en los modos **SONG**, **VOICE**, **UTILITY** y **RECORD**. El indicador central muestra la página actual y el total.

### TEMPO / TAP

Pulsa **TEMPO / TAP** para editar el BPM con DATA. También puedes pulsarlo cuatro veces siguiendo un ritmo y el simulador calculará el tempo aproximado.

### RECORD

1. Pulsa **RECORD**.
2. Selecciona una canción de usuario entre 51 y 54.
3. Avanza con **PAGE +** hasta `RECORD READY`.
4. Pulsa **START / STOP** y toca los pads.
5. Pulsa nuevamente **START / STOP** para finalizar.
6. Vuelve a pulsarlo para reproducir lo grabado.

## Ajustar el volumen de un instrumento

El volumen de cada pad se guarda por separado. Modificar SNARE no cambia KICK, los toms ni los platos.

1. Golpea el pad que quieres modificar.
2. Pulsa **VOICE**.
3. Avanza con **PAGE +** hasta `VOLUME / PAN`.
4. Comprueba que el cursor `>` esté colocado sobre `Vol`.
5. Gira **DATA** para subir o bajar el volumen.
6. Golpea otro pad para comprobar que conserva su propio valor.

## Ajustar la sensibilidad

1. Golpea el pad que quieres usar como referencia.
2. Pulsa **UTILITY**.
3. Avanza con **PAGE +** hasta `GAIN / M.VEL`.
4. Selecciona `Gain` y gira **DATA**.
5. Avanza a `VELOCITY CURVE` para elegir la respuesta deseada.
6. Vuelve a tocar el pad y compara el resultado.

Una ganancia mayor facilita la respuesta a golpes suaves. Conviene aumentarla gradualmente para evitar dobles disparos.

## Guías de aprendizaje

| N.º | Práctica |
|---:|---|
| 1 | Encendido y volumen general |
| 2 | Aprender a usar DATA |
| 3 | Elegir y probar un kit |
| 4 | Volumen de cada instrumento |
| 5 | Sensibilidad y respuesta |
| 6 | Tempo y metrónomo |
| 7 | Asignar una voz y guardar |
| 8 | Grabar y reproducir |

Las guías avanzan únicamente cuando se realiza la acción solicitada. El botón **Reiniciar progreso** vuelve el curso a `0/8`.

## Panel trasero

La vista **Conexiones** representa:

- MIDI IN y MIDI OUT de 5 pines.
- Ocho entradas de disparo para los pads.
- Entrada para el control del Hi-Hat.
- AUX IN.
- AUX OUT L/MONO y AUX OUT R.
- Entrada de alimentación DC IN 9V.

## Archivos del proyecto

```text
simulador-interactivo-DD-602-DD-1000/
├── index.html   # Abre el simulador
├── app.js       # Lógica y componentes compilados
├── app.css      # Diseño y adaptación visual
├── LEEME.txt    # Instrucciones rápidas
└── README.md    # Documentación del repositorio
```

## Publicarlo con GitHub Pages

1. Entra en **Settings** dentro del repositorio.
2. Abre la sección **Pages**.
3. En `Build and deployment`, elige **Deploy from a branch**.
4. Selecciona la rama `main` y la carpeta `/ (root)`.
5. Pulsa **Save** y espera a que GitHub genere el enlace.

## Versión 1.4

- Rueda DATA ampliada, más visible y con giro animado.
- Signos `−` y `+` realineados.
- Ocho guías esenciales completamente renovadas.
- Progreso corregido y reiniciable.
- Volumen independiente por instrumento.
- Sensibilidad y curva de velocidad con efecto audible.
- Panel trasero corregido según el manual.
- Mejoras en PAGE, TEMPO / TAP y RECORD.

## Solución de problemas

### No se escucha nada

Pulsa **POWER** y sube **MAIN VOLUME**. Algunos navegadores bloquean el audio hasta que el usuario hace clic por primera vez dentro de la página.

### DATA no cambia el valor

Primero selecciona un modo o parámetro editable, como **KITS**, **TEMPO**, **VOICE** o **UTILITY**.

### Las guías aparecen completadas

Pulsa **Reiniciar progreso** en el panel izquierdo para volver a `0/8`.

## Tecnologías

- HTML5
- CSS3
- JavaScript
- React y TypeScript en el código fuente original
- Web Audio API para la recreación didáctica de los sonidos

## Aviso

Este proyecto es una herramienta educativa independiente. El audio es una recreación generada por el navegador y no una emulación exacta del hardware. Los nombres y referencias del DD-602 / DD-1000 se utilizan únicamente con fines formativos.

---

Desarrollado por [antibata](https://github.com/antibata).
