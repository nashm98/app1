# Memora

Juego web tipo ahorcado con **20 niveles**, tiempo limitado y progreso por puntos.

## Cómo jugar

1. Abre `index.html` en tu navegador.
2. En cada nivel hay **un único campo de ingreso** y un botón (`▶`):
   - Si escribes 1 carácter, se toma como intento de letra.
   - Si escribes más de 1 carácter, se toma como intento de palabra completa.
3. Usa el selector de idioma con bandera + texto (**🇪🇸 Español, 🇬🇧 English, 🇵🇹 Português**).
4. Usa el botón ☀️/🌙 para alternar entre modo día y modo nocturno.

## Reglas clave

- Para pasar de nivel debes **acumular puntos** (varias palabras correctas), no solo acertar una.
- Cada palabra acertada suma 1 punto al progreso del nivel.
- El tiempo comienza en la **primera acción** (probar intento o pulsar algún botón).
- Letra correcta: revela posiciones y suma tiempo extra.
- Letra incorrecta: descuenta 1 intento.
- Palabra incorrecta: descuenta 1 intento.
- Botón de pista: muestra `Pista:` / `Hint:` / `Dica:` y descuenta 1 intento.

## Generación de palabras

- **Modo online**: intenta obtener palabras aleatorias desde APIs públicas.
- **Cache anti-repetición**: evita repetir palabras durante la sesión por idioma.
- **Fallback offline**: si falla la conexión/API, usa automáticamente el pool local del nivel.
- Las palabras y pistas se adaptan al idioma elegido (es/en/pt).

## Popup de resultado

- Al acertar una palabra: aparece popup con pista/definición y opción para continuar.
- Al completar los puntos del nivel: aparece popup de **Nivel superado** para avanzar.
- Al perder: aparece popup para **Comenzar de nuevo**.
