# 🌱 De Cero a Código

**Juego para aprender JavaScript desde cero, programando un robot jardinero.**

Escribes JavaScript de verdad, pulsas Ejecutar y Robi obedece al instante: camina, gira y planta
flores. El juego comprueba tu código solo: 9 niveles, 3 pistas por nivel, solución explicada y
estrellas.

---

## 1. Qué es

Un juego educativo de navegador (HTML + CSS + JavaScript) en el que el jugador **programa de
verdad**, no con un lenguaje inventado: el código que escribes es JavaScript y lo ejecuta el
navegador.

Lo que se aprende, en este orden:

- **Funciones y orden**: una instrucción por línea, de arriba abajo.
- **Bucles** `for`: repetir sin copiar y pegar.
- **Variables** `let`: guardar un valor con nombre.
- **Giros y direcciones**: pensar el movimiento paso a paso.
- **Condicionales** `if`: decidir cuándo hacer algo.
- **Funciones propias**: escribir un bloque una vez y reutilizarlo.
- **Bucles anidados**: repetir una fila dentro de otra.
- **Listas (arrays)** y `for...of`: varios valores juntos.

No hay que instalar nada, no hay dependencias ni servidor, y no se envía ningún dato a ninguna
parte: todo ocurre en tu navegador.

**Para quién es:** para quien empieza desde cero (a partir de ~10–12 años) y quiere aprender
programación de verdad, y también para quien ya programa en otro lenguaje y quiere calentar.

**Duración:** entre 40 y 70 minutos para los 9 niveles.

---

## 2. Cómo se abre

| Formato | Qué abrir | Cuándo usarlo |
|---|---|---|
| Un solo archivo | `de-cero-a-codigo.html` | Lo más rápido: doble clic y a jugar. |
| Carpeta | `primer-codigo/index.html` | Si quieres leer o modificar el código del juego. |

Funciona en cualquier navegador moderno (Chrome, Edge, Firefox, Safari) en ordenador, tableta y
móvil. **No necesita conexión a internet** en ningún momento.

---

## 3. La pantalla

    ┌──────────────┬───────────────────────┬────────────────────────┐
    │  MISIÓN      │   🌱 EL JARDÍN        │   EDITOR               │
    │  qué hay que │   Robi se mueve aquí  │   aquí escribes JS     │
    │  hacer       │   al ejecutar         │   ────────────────     │
    │  objetivos ✓ │   velocidad · reinicio│   CONSOLA (mensajes)   │
    │  pistas 💡   │   leyenda             │                        │
    └──────────────┴───────────────────────┴────────────────────────┘

- **Misión**: el reto, los objetivos (se marcan solos) y las pistas.
- **Jardín**: la cuadrícula con Robi 🤖, las casillas marcadas ⭕ (donde hay que plantar), las
  flores 🌸 y las rocas 🪨. Debajo: velocidad de la animación y botón para reiniciar el jardín.
- **Editor**: tu código. Debajo, la **consola**, donde salen los mensajes, los errores y el
  número de línea cuando algo falla.

**Arriba** están los 9 niveles: puedes volver a cualquiera que ya hayas abierto.

---

## 4. Los comandos de Robi

Todo se escribe como una llamada con paréntesis: `comando()`.

| Comando | Qué hace |
|---|---|
| `avanzar()` | Mueve a Robi una casilla hacia delante. |
| `avanzar(3)` | Lo mueve 3 casillas de golpe. |
| `girarDerecha()` | Gira a la derecha sin cambiar de casilla. |
| `girarIzquierda()` | Gira a la izquierda sin cambiar de casilla. |
| `plantar()` | Planta una flor en la casilla donde está Robi. |
| `faltaFlor()` | Pregunta: ¿esta casilla necesita flor? (sí / no) |
| `hayFlor()` | Pregunta: ¿ya hay flor aquí? |
| `hayRoca()` | Pregunta: ¿hay una roca justo delante? |
| `decir("hola")` | Escribe un mensaje en la consola, precedido de «Robi dice:». |

Robi empieza siempre **mirando a la derecha** de la pantalla, así que un giro a la derecha lo deja
mirando hacia **abajo**. Las rocas no se pueden atravesar.

---

## 5. Cómo se juega

1. Lee la misión y mira el jardín: las casillas con **círculo** son las que necesitan flor.
2. Escribe tu código en el editor.
3. Pulsa **▶ Ejecutar** (o `Ctrl + Enter`). El código se ejecuta de verdad y el jardín se anima
   paso a paso.
4. El juego mira el resultado:
   - Si **todas las casillas marcadas tienen flor y no sobra ninguna**, nivel superado.
   - Si falta alguna, te dice cuántas; si sobra, te avisa de las flores de más;
   - si Robi choca con una roca o se sale del jardín, el error sale en la consola con su línea.
5. Pasa al siguiente nivel, o repite para conseguir las 3 estrellas.

Detalle importante: **la flor solo cuenta en las casillas marcadas**. Plantar en cualquier sitio
no es un fallo del juego, es un fallo del plan: por eso en el nivel 5 hay que aprender a decidir
con `if`.

---

## 6. Los 9 niveles

| # | Nivel | Se aprende | Reto |
|---|-------|-----------|------|
| 1 | Tu primer código | funciones y orden | 2 flores seguidas |
| 2 | El bucle que repite | `for` | 4 flores sin copiar líneas |
| 3 | Una caja llamada variable | `let` | 5 flores con un número guardado |
| 4 | Aprender a girar | giros y direcciones | una columna de 3 flores |
| 5 | Decidir con `if` | condicional + `faltaFlor()` | plantar solo donde toca |
| 6 | Tu propia función | `function` y llamadas | 6 flores en dos filas |
| 7 | Bucles dentro de bucles | anidados | un cuadrado de 9 flores |
| 8 | Listas de números | arrays y `for...of` | distancias 1, 3, 3 |
| 9 | El jardín imposible | todo junto | rodear un muro, 2 flores |

---

## 7. Ayudas

- **💡 Dame una pista** — 3 pistas por nivel, de menos a más: *la idea* → *cómo se escribe* →
  *código casi completo con huecos*.
- **🧪 Ver la solución** — el código final **explicado** y un botón para copiarlo al editor y
  verlo funcionar.
- **Botón `?`** (arriba a la derecha) — recordatorio de todos los comandos y de lo que se aprende.
- **Velocidad** (lenta / normal / rápida) — para ver el recorrido paso a paso o ir directo al
  resultado. Con muchas acciones el juego acelera solo.
- **↺ Reiniciar jardín** — limpia el tablero sin tocar tu código.
- **Consola** — los mensajes de `decir()`, los errores y la línea donde están.

---

## 8. Puntuación y progreso

- **⭐⭐⭐** superar el nivel sin usar pistas.
- **⭐⭐** con 1 o 2 pistas. **⭐** con las 3 pistas.
- El progreso **y el código de cada nivel** se guardan en el navegador (clave
  `dczc-progreso-v1` en `localStorage`). Al cerrar y volver, sigues donde estabas.
- Para empezar de cero: borra los datos del sitio en el navegador o usa una ventana privada.
- Los niveles se pueden repetir; se conserva la mejor puntuación.

---

## 9. Errores típicos (y qué te dice el juego)

| Lo que pasa | Lo que ves en la consola |
|---|---|
| Se acaba la cuadrícula | *¡Robi se sale del jardín! Gíralo antes de seguir avanzando.* |
| Hay una roca delante | *¡Hay una roca delante! Rodéala con giros.* |
| Flor fuera de sitio | *Hay N flor(es) donde no tocaba 🥀* |
| Faltan flores | *¡Casi! Faltan N flor(es).* |
| Se olvidó un paréntesis o una llave | *Falta cerrar un paréntesis, una llave o un corchete.* + línea marcada |
| `avanzar(0)` o un valor raro | *avanzar() necesita un número mayor que 0. Ejemplo: avanzar(3)* |
| Bucle que no termina | *¡Demasiadas acciones! Robi se ha cansado…* |
| Nombre mal escrito (`avanzr()`) | Error de JavaScript con el número de línea |

Receta si te atascas: lee el objetivo → mira la consola → pide **una** pista → mira la solución y
al día siguiente escríbela de memoria.

---

## 10. Cómo funciona por dentro (para curiosos y docentes)

- El código del jugador se ejecuta **de verdad** con `new Function`, recibiendo como parámetros
  los comandos (`avanzar`, `plantar`…). No hay intérprete propio ni traducción: es JavaScript.
- Antes de ejecutar, cada comando registra lo que ocurre; después la interfaz **reproduce** esa
  lista de acciones animando el jardín. Por eso se puede cambiar la velocidad sin cambiar el
  resultado.
- **Seguridad**: el bucle `while` (y `do`) está bloqueado a propósito, porque un bucle infinito
  congelaría la pestaña; se avisa con un mensaje y se propone `for`. Además hay un tope de 600
  acciones por ejecución.
- Los errores de sintaxis se detectan contando paréntesis, llaves y corchetes, para poder señalar
  una línea probable, y la línea del error se resalta en el margen del editor.
- Todo el estado del juego está en `localStorage`: no hay cuentas, ni red, ni analítica.

**Para usar en clase:** los niveles 1–4 son una sesión, los 5–7 otra y los 8–9 una tercera. Las
pistas están graduadas para que nadie se quede bloqueado, y el botón de solución sirve para
explicar en la pizarra.

---

## 11. Archivos del juego

    primer-codigo/
    ├── index.html     interfaz (misión, jardín, editor)
    ├── estilos.css    aspecto visual del juego
    ├── juego.js       niveles + comandos de Robi + comprobación
    └── README.md      este archivo

Los 9 niveles están en un array (`NIVELES`) dentro de `juego.js`, dibujados como pequeñas
cuadrículas de texto:

    "R**......"     R = Robi   * = casilla marcada
    "........."     # = roca   . = suelo

Para **añadir un nivel** basta con copiar uno parecido, cambiar el `id`, el mapa, el texto y las
pistas. La comprobación no depende del nivel: siempre es «todas las casillas marcadas con flor y
ninguna flor de más».

---

## 12. Preguntas frecuentes

**¿Necesito internet?** No. Ni para jugar, ni para guardar el progreso.

**¿Es JavaScript de verdad?** Sí. `for`, `let`, `if`, funciones, arrays y `for...of` son
JavaScript estándar; lo único especial son los comandos de Robi.

**¿Se puede jugar en el móvil?** Sí, se puede escribir y ejecutar, aunque programar en el móvil es
incómodo: mejor tableta u ordenador.

**¿Por qué no puedo usar `while`?** Para que la página nunca se quede colgada. Con `for` se hace
lo mismo y siempre tiene final.

**No me guarda el progreso.** Pasa en ventanas privadas o si el navegador bloquea el
almacenamiento local; el juego funciona igual, empezando de cero.

**¿Y el juego de HTML y CSS?** *«El Teatro del Código»*: 14 niveles para aprender etiquetas,
selectores y propiedades. Los dos son independientes.

---

*Hecho para aprender programando de verdad. Si algo no se ve bien en tu navegador, avísame y se
corrige.*
