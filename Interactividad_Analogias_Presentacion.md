# Brief de Interactividad — Dos Analogías del Modelo Consultivo
**Para:** Implementación por IA / desarrollador
**Contexto:** Material de presentación interna Ingenia Latam · 18 marzo 2026
**Propósito:** Dos módulos interactivos independientes para mostrar el contraste entre el modelo publicitario tradicional y el modelo consultivo de Ingenia. Se presentan en secuencia durante la reunión.

---

## MÓDULO 1 — La Analogía del Fútbol

### Concepto narrativo

El modelo publicitario viejo funciona como el fútbol de antes: los delanteros se quedan arriba esperando la bola. Cada uno defiende o ataca por separado. Todo el mundo corre la bola sin sistema.

El modelo consultivo funciona como el fútbol moderno: cuando atacas, atacas en bloque. Cuando defiendes, defiendes en bloque. Duplas, pases limpios, fricción constante que eleva la calidad.

---

### Estructura de pantallas

#### Estado A — "El modelo publicitario" (pantalla inicial)
**Encabezado:** `El modelo de agencia`
**Subtítulo:** *Cada quien espera su turno*

**Visualización (cancha de fútbol simplificada, vista desde arriba):**
```
[ARCO RIVAL]

  ⚽ ⚽ ⚽      ← Delanteros (creativos) esperando la bola arriba
                  Inmóviles. Pasivos. "Pásenme el trabajo."


  🔄 🔄 🔄     ← Zona media: todos corretean la misma bola
                  Cuentas, strategy, arte — sin dirección clara


  🔄 🔄        ← Defensa (admin, ops) reaccionando a lo que llega

[ARCO PROPIO]
```

**Etiquetas al costado o debajo de cada grupo:**
- Delanteros → *"Creativos esperando el brief"*
- Zona media → *"Todos hacen de todo, nadie tiene foco"*
- Defensa → *"Reaccionando, nunca anticipando"*

**Texto descriptivo (pequeño, debajo):**
> *En el modelo de agencia, el delantero espera que le pasen la bola. El modelo funciona en modo reactivo: cada área espera que otra le "pase el trabajo". Resultado: desconexión, reprocesos, pérdida de calidad.*

---

#### Estado B — "El modelo consultivo" (al hacer clic/toggle)
**Encabezado:** `El modelo consultivo`
**Subtítulo:** *Trabajo en bloque · Duplas · Fricción que eleva la calidad*

**Visualización (misma cancha, diferente formación):**
```
[ARCO RIVAL]

  ↑ ↑ ↑ ↑ ↑ ↑  ← ATAQUE EN BLOQUE — todos suben
  ↑ ↑ ↑ ↑ ↑ ↑    Estrategia + Creativo + Cuentas + Digital
                   Duplas activas, pases limpios, foco compartido


  (posición media organizada)


  ↓ ↓ ↓ ↓ ↓ ↓  ← DEFENSA EN BLOQUE — todos bajan y protegen
  ↓ ↓ ↓ ↓ ↓ ↓    Ops protege el modelo · Admin protege el margen

[ARCO PROPIO]
```

**Etiquetas de duplas (iconos conectados por líneas):**
- `Estrategia ↔ Growth Digital`
- `Dir. Creativo ↔ Dir. de Arte`
- `Redactor Sr ↔ Diseñador Sr`
- `Operaciones ↔ Ejecutivas`

**Texto descriptivo:**
> *En el modelo consultivo, nadie espera. Todos se mueven en bloque. Cuando hay un brief, estrategia y creativo trabajan juntos desde el inicio. Los pases son limpios. La fricción entre roles eleva la calidad — no la dispersa.*

---

### Mecánica de interacción

- **Trigger:** botón toggle o swipe horizontal entre Estado A y Estado B
- **Transición:** animación de los puntos (jugadores) moviéndose de una formación a la otra
- **Duración animación:** 800ms, suave (ease-in-out)
- **Elemento visual destacado:** una pelota que en el Estado A va en zigzag caótico; en el Estado B va de jugador a jugador en líneas limpias
- **Botón:** `← Ver modelo agencia` / `Ver modelo consultivo →`

---

### Texto de cierre (aparece debajo de ambos estados)

> *La diferencia no es quién trabaja más. Es si el equipo trabaja en sistema o en modo reactivo.*

---

---

## MÓDULO 2 — La Analogía de las Postas 4×100

### Concepto narrativo

En las postas 4×100, cada corredor hace su parte de la carrera y luego entrega el bastón al siguiente. Si le entregas mal la posta al siguiente corredor — le tiras el bastón a media altura, a mala velocidad, fuera de zona — **la carrera está perdida**, aunque él corra perfecto.

En el modelo consultivo, cada rol hace lo mismo:
- Si el **Planner** entrega mal el insight → la estrategia sale torcida
- Si la **Estrategia** entrega mal el brief → el creativo trabaja sin dirección
- Si el **Creativo** entrega mal la plataforma → el Arte no puede construir el sistema visual
- Si el **Arte** entrega mal los assets → el despliegue pierde impacto

Cada uno hace su rol con calidad porque sabe que el siguiente depende de eso.

---

### Estructura de pantallas

#### Pantalla base — La pista
**Encabezado:** `¿Qué pasa si entregas mal la posta?`

**Visualización (pista de atletismo, vista lateral, 4 carriles):**

```
INICIO ──────────────────────────────────────────── META

  🏃  ZONA 1     →  [POSTA]  →    🏃  ZONA 2    →  [POSTA]  →  🏃  ZONA 3  →  [POSTA]  →  🏃  ZONA 4  →  🏆
 Planner Jr               Estrategia             Dir. Creativo             Dir. de Arte         Despliegue
 Insights &               Marco +                Plataforma                Sistema              Campaña
 Research                 Brief                  Creativa                  Visual               Final
```

**Estado inicial:** los 4 corredores en posición, pistas iluminadas, bastones en mano. Todo verde.

---

#### Interacción — Hacer clic en cada "zona de posta" (los 3 puntos de entrega)

**Al hacer clic en cada bastón, se despliega un panel con dos opciones:**

---

**POSTA 1: Planner Jr → Estrategia**

*Si la entrega sale BIEN (clic en "✅ Posta limpia"):*
```
Insight: "El cliente no tiene problema de visibilidad — tiene problema de confianza del segmento B2B"
→ La estrategia tiene el problema real. Construye sobre datos sólidos.
→ PISTA: se ilumina en verde hacia adelante
```

*Si la entrega sale MAL (clic en "⚠️ Posta sucia"):*
```
Insight: "El cliente quiere más awareness"
→ La estrategia trabaja sobre el síntoma, no el problema real.
→ El brief creativo nace torcido. Todo lo que sigue... está mal orientado.
→ PISTA: se ilumina en rojo. Los corredores siguientes se ralentizan visualmente.
```

---

**POSTA 2: Estrategia → Dir. Creativo**

*Si la entrega sale BIEN:*
```
Brief: Problema real + tensión + criterio BECD + tipología de campaña
→ El creativo sabe exactamente qué resolver y con qué restricciones.
→ La plataforma creativa nace defendible.
→ PISTA: verde, velocidad normal
```

*Si la entrega sale MAL:*
```
Brief: "Algo moderno, que impacte, con mucho color"
→ El Director Creativo inventa dirección porque no tiene marco.
→ La plataforma no se puede defender en comité.
→ PISTA: roja. Corredor frena. Tiempo perdido en correcciones.
```

---

**POSTA 3: Dir. Creativo → Dir. de Arte**

*Si la entrega sale BIEN:*
```
Plataforma: Territorio + concepto madre + criterios de campaña
→ Arte construye un sistema visual coherente con la narrativa.
→ Escala sin inconsistencias.
→ META: carrera ganada 🏆
```

*Si la entrega sale MAL:*
```
Plataforma: "Algo inspirado en naturaleza y tecnología"
→ Arte diseña sin dirección conceptual clara.
→ El sistema visual no tiene coherencia con la estrategia.
→ La campaña llega al cliente sin hilo conductor.
→ META: carrera perdida ❌
```

---

#### Estado final — "Carrera completada"

**Si todas las postas fueron limpias:**
```
🏆 CARRERA GANADA

Resultado: La campaña llega al cliente alineada.
Estrategia + Creatividad + Arte + Despliegue = coherencia total.
El cliente percibe profundidad, no piezas aisladas.
```

**Si alguna posta fue sucia:**
```
❌ CARRERA PERDIDA

Resultado: [nombre del rol que falló] entregó mal la posta.
El equipo después corrió perfecto — pero ya era tarde.
La calidad del entregable final depende de la calidad de cada entrega.
```

---

### Mecánica de interacción

- **Trigger principal:** clic en cada "zona de entrega" (bastón entre corredores)
- **En cada bastón:** despliega un panel con dos opciones — `✅ Posta limpia` / `⚠️ Posta sucia`
- Al elegir una opción, la pista se colorea (verde/rojo) desde ese punto hacia adelante
- El usuario puede explorar los tres bastones en cualquier orden
- **Botón de reset:** "Volver a empezar la carrera"
- **Opcional:** modo "historia guiada" que muestra la secuencia completa automáticamente

---

### Variante de uso en presentación (modo demo)

Para usar en la reunión sin que el equipo interactúe solo:

1. JC muestra la pista base con todos los corredores
2. Hace clic en el bastón 2 (Estrategia → Creativo) y elige "Posta sucia"
3. La pista se vuelve roja hacia adelante
4. Pregunta al equipo: *"¿Qué le pasa al Director Creativo si le llega este brief?"*
5. Escucha respuestas
6. Luego hace la posta limpia → la pista se vuelve verde
7. Cierre: *"La calidad de lo que produces no depende solo de ti. Depende de qué tan bien le pasas la posta al siguiente."*

---

## Especificaciones técnicas para el AI que lo implementa

### Stack sugerido
- **React** con hooks (useState para gestionar estados de cada módulo)
- **Tailwind CSS** para estilos inline
- **Lucide React** para íconos si aplica
- No requiere backend ni localStorage

### Paleta de colores (Ingenia)
- Naranja Ingenia: `#FF6B00` o similar
- Verde posta limpia: `#22C55E`
- Rojo posta sucia: `#EF4444`
- Fondo neutro: `#F8F8F8` o `#FFFFFF`
- Texto: `#1A1A1A`

### Entregable esperado
- Componente React `.jsx` con ambos módulos
- Módulo 1 y Módulo 2 en la misma página, separados visualmente
- Navegación simple entre los dos (tabs o scroll)
- Funciona en pantalla de laptop (1280px+)
- Sin dependencias externas más allá de las disponibles (React, Tailwind, Lucide)

---

*Brief de interactividad · Analogías del modelo consultivo · Ingenia Latam · Marzo 2026*
