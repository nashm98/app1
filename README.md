# Memora

Juego web tipo ahorcado con **20 niveles**, tiempo limitado y progreso por puntos.

## Cómo jugar

1. Abre `index.html` en tu navegador.
2. En cada nivel hay **un único campo de ingreso** y un botón (`Probar intento`):
   - Si escribes 1 carácter, se toma como intento de letra.
   - Si escribes más de 1 carácter, se toma como intento de palabra completa.

## Reglas clave

- Para pasar de nivel debes **acumular puntos** (varias palabras correctas), no solo acertar una.
- Cada palabra acertada suma 1 punto al progreso del nivel.
- Las palabras de cada nivel se eligen de forma **aleatoria**.
- El tiempo comienza en la **primera acción** (probar intento o pulsar algún botón).
- Letra correcta: revela posiciones y suma tiempo extra.
- Letra incorrecta: descuenta 1 intento.
- Palabra incorrecta: descuenta 1 intento.
- Usar **PISTA**: muestra ayuda y descuenta 1 intento.

## Popup de resultado

- Al acertar una palabra: aparece popup con definición y opción para continuar.
- Al completar los puntos del nivel: aparece popup de **Nivel superado** para avanzar.
- Al perder: aparece popup para **Comenzar de nuevo**.
