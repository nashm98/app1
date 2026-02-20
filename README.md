# app1

Juego web tipo ahorcado con **20 niveles de dificultad** y tiempo limitado.

## Cómo jugar

1. Abre `index.html` en tu navegador.
2. En cada nivel hay **un único campo de ingreso** y **un solo botón** (`Probar intento`):
   - Si escribes 1 carácter, se toma como intento de letra.
   - Si escribes más de 1 carácter, se toma como intento de palabra completa.
3. Reglas:
   - El tiempo comienza en la **primera acción** (probar intento o pulsar algún botón).
   - Letra correcta: revela posiciones y suma tiempo extra.
   - Letra incorrecta: descuenta 1 intento.
   - Palabra incorrecta: descuenta 1 intento y muestra definición de la palabra del nivel.
   - Intento de palabra (acierto o fallo): muestra definición/uso de la palabra del nivel.
   - Al perder o al superar el nivel, también se muestra la definición de la palabra del nivel.
   - Usar **PISTA**: muestra ayuda y descuenta 1 intento.
4. Al completar un nivel, usa **Siguiente nivel** hasta llegar al 20.

## Dificultad y temáticas

- Los primeros niveles usan palabras cotidianas.
- Luego aumentan longitud y complejidad conceptual.
- Las temáticas son variadas: hogar, ciudad, naturaleza, ciencia, historia, lengua, finanzas, educación y más.
