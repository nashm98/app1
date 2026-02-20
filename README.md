# Memora

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
   - Palabra incorrecta: descuenta 1 intento.
   - Usar **PISTA**: muestra ayuda y descuenta 1 intento.
4. Al perder o superar nivel, aparece un **popup** con la definición de la palabra:
   - Si ganas: muestra “Nivel superado” y permite avanzar.
   - Si pierdes: muestra cartel para **comenzar de nuevo**.
