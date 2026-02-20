# Memora

Juego web tipo ahorcado con **20 niveles**, tiempo limitado y progreso por puntos.

## Cómo jugar

1. Abre `index.html` en tu navegador.
2. En cada nivel hay **un único campo de ingreso** y un botón (`▶`):
   - Si escribes 1 carácter, se toma como intento de letra.
   - Si escribes más de 1 carácter, se toma como intento de palabra completa.
3. Usa el selector de idioma con bandera + texto (**🇪🇸 Español, 🇬🇧 English, 🇵🇹 Português**).
4. Usa el selector deslizante tipo perilla para alternar entre modo día y modo nocturno.
5. Los popups de resultado también respetan el tema seleccionado (claro/oscuro).
6. El fondo incluye tramas sutiles variables para dar dinamismo sin afectar legibilidad.

## Reglas clave

- Para pasar de nivel debes **acumular puntos** (varias palabras correctas), no solo acertar una; el objetivo de puntos sube progresivamente por nivel.
- La complejidad de palabra aumenta con el nivel, pero con longitudes variadas dentro de cada nivel para mayor aleatoriedad.
- Cada palabra acertada suma 1 punto al progreso del nivel.
- Si aciertas una palabra sin usar pistas, recibes 1 punto extra de bonificación.
- El tiempo comienza en la **primera acción** (probar intento o pulsar algún botón).
- Letra correcta: revela posiciones y suma tiempo extra.
- Letra incorrecta: descuenta 1 intento y activa una animación breve de vibración/destello rojo.
- Palabra incorrecta: descuenta 1 intento.
- Botón de pista: permite hasta 5 pistas por palabra y resta puntos acumulados: `-1`, `-3`, `-5`, `-7`, `-9`.
- No se permiten puntos negativos: si no alcanzan los puntos para una pista, se bloquea con mensaje de puntos insuficientes.
- Para pedir desde la 2ª pista en adelante, primero debes acertar al menos una letra.
- Las pistas se muestran en varios niveles con frases completas y más específicas por palabra (categoría útil, forma de la palabra, vocales, letra media y pista completa).

## Generación de palabras

- **Modo online**: intenta obtener palabras aleatorias desde APIs públicas en inglés.
- En **español** se fuerza el vocabulario local del juego para evitar que aparezcan palabras en inglés.
- **Diccionario ampliado**: se añadieron más palabras por nivel (especialmente en español) para reducir repeticiones.
- **Cache anti-repetición**: evita repetir palabras durante la sesión por idioma.
- **Fallback offline**: si falla la conexión/API, usa automáticamente el pool local del nivel.
- Las palabras y pistas se adaptan al idioma elegido (es/en/pt), usando vocabulario local en español y portugués para mantener consistencia.
- También se respeta un rango de longitud por nivel para sostener una progresión de dificultad más clara.

## Popup de resultado

- Al acertar una palabra: aparece popup con pista/definición y opción para continuar.
- Al completar los puntos del nivel: aparece popup de **Nivel superado** para avanzar.
- Al perder: aparece popup para **Comenzar de nuevo**.
