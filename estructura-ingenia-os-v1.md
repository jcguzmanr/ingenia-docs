# Ingenia OS — Estructura del Sistema Operativo Consultivo v1

> Documento de referencia para alineación interna.
> Este documento describe la estructura actual, el razonamiento detrás de cada decisión,
> y el objetivo de convergencia con los inputs estratégicos de Luis Holder.

---

## 1. La estructura actual

```
🟠 Ingenia/
│
├── .claude/                         ← configuración del sistema AI
│   ├── CLAUDE.md                    ← instrucciones globales
│   └── rules/                       ← reglas modulares por dominio
│       ├── método.md                ← cómo operar según modelo 1→4
│       ├── clientes.md              ← reglas de carpeta cliente
│       ├── pipeline.md              ← reglas de prospección
│       └── herramientas.md          ← sync de automatizaciones
│
├── CLAUDE.md                        ← mapa general del proyecto
├── TASKS.md                         ← registro vivo de tareas
├── PRIORITIES.md                    ← jerarquía de tipos de trabajo
│
├── _método/                         ← framework Foundational (fuente de verdad)
│   ├── fundacionales/
│   │   ├── originales/              ← PDFs, DOCXs fuente
│   │   └── destilados/              ← .md y .html procesados
│   ├── 1-negocio/
│   ├── 2-marca/
│   ├── 3-comunicación/
│   └── 4-creatividad/
│
├── _clientes/                       ← clientes activos
│   └── [cliente]/
│       ├── README.md
│       ├── 1-negocio/
│       ├── 2-marca/
│       ├── 3-comunicación/
│       ├── 4-creatividad/
│       └── _entregables/
│
├── _pipeline/                       ← prospectos pre-cliente
│   └── [prospecto]/
│       └── README.md
│
├── _operación/                      ← máquina interna
│   ├── clickup/
│   ├── procesos/
│   ├── reportes/
│   └── comités/
│
├── _conocimiento/                   ← IP acumulada
│   ├── industrias/
│   ├── casos/
│   └── research/
│
├── _herramientas/                   ← tools del sistema
│   ├── automatizaciones/
│   ├── skills/
│   ├── templates/
│   ├── prompts/
│   └── dashboards/
│
└── _inbox/                          ← zona de triage
```

---

## 2. Cómo llegamos a esta estructura

### Punto de partida

La carpeta Ingenia comenzó como un repositorio plano donde coexistían
carpetas de gestión (Dani), material de Luis Holder, documentos del
modelo consultivo, clientes, pipeline, plan de 90 días y dashboards —
todo en el mismo nivel, sin jerarquía ni convención de nombres.

### Problemas que resolvimos

**Fragmentación del método.** Los documentos fundacionales del Modelo
Consultivo estaban dispersos en 3 carpetas distintas (_Proceso Consultivo,
Modelo Consultivo y Procesos, Plan 90 dias). No había un solo lugar
donde ir a consultar "el método". Ahora viven en `_método/fundacionales/`
con separación entre originales y destilados.

**Clientes sin estructura espejo.** Las carpetas de clientes no reflejaban
las 4 fases del modelo. Ahora cada cliente replica la secuencia
1-negocio → 2-marca → 3-comunicación → 4-creatividad. Las carpetas
vacías comunican "fase no iniciada" — no hace falta leer nada para
saber en qué punto está un cliente.

**Pipeline desconectado del método.** El pipeline vivía como proceso
puramente comercial. Ahora cada prospecto documenta en qué fase del
método entraría, conectando venta con consultoría desde el primer
contacto.

**Sin lugar para conocimiento reutilizable.** Los insights de industria,
casos internos y research estratégico se perdían dentro de carpetas de
clientes. `_conocimiento/` centraliza la IP que no pertenece a un
cliente específico.

**Herramientas invisibles.** Las automatizaciones (scheduled tasks),
los skills del AI, los templates y dashboards no tenían presencia en
la estructura. `_herramientas/` les da visibilidad con inventario,
changelogs y mecanismo de sincronización automática.

**Sin triage.** Los archivos nuevos no tenían destino claro. `_inbox/`
es la zona donde cae todo lo sin clasificar con regla de 48 horas
máximo de permanencia.

### Principios de diseño

1. **El método es el eje.** La secuencia 1→2→3→4 se refleja en la
   estructura de carpetas, no solo en los documentos.

2. **Cada carpeta raíz tiene un rol semántico.** No hay carpetas genéricas.
   El prefijo `_` indica carpetas estructurales del sistema.

3. **README.md como metadata.** Cada subcarpeta tiene un README que
   funciona como tarjeta de estado: fase, equipo, siguiente acción.

4. **Rules como configuración viva.** Las reglas en `.claude/rules/`
   no son documentación — son instrucciones operativas que el AI
   ejecuta en cada sesión.

5. **Progresivo, no big bang.** La estructura se construye por capas.
   Las carpetas vacías son intencionales — se llenan cuando hay
   contenido real.

---

## 3. Dónde vive esta estructura

| Capa | Función | Estado |
|---|---|---|
| **Local** | Cockpit operativo. Es donde el AI opera con máximo detalle, ejecuta automatizaciones, genera entregables y mantiene el inventario sincronizado. | Activo ✓ |
| **Google Drive** | Redundancia y acceso compartido. Replica la estructura para que el equipo pueda consultar sin depender del entorno local. | Pendiente de configurar |
| **ClickUp** | Gestión de tareas y visibilidad ejecutiva. No reemplaza la estructura de archivos — la complementa con seguimiento de estado, asignaciones y timelines. | En implantación |

La estructura de carpetas y ClickUp no compiten. Cada capa tiene un rol:

- **Archivos** (Local/Drive) = qué se produjo, el conocimiento, los entregables
- **ClickUp** = quién hace qué, cuándo, en qué estado está

---

## 4. Cómo se conecta con el Modelo Consultivo Foundational

```
         _método/ (fuente de verdad)
              │
    ┌─────────┼─────────┐
    │         │         │
_clientes/  _pipeline/  _conocimiento/
    │         │         │
    └─── cada uno referencia ───┘
         las 4 fases del método
```

- `_método/` contiene el framework puro: documentos fundacionales,
  guías por fase, templates de referencia.
- `_clientes/` instancia el método: cada cliente tiene carpetas de fase
  que reflejan dónde están en el proceso.
- `_pipeline/` conecta la venta con el método: cada prospecto mapea
  en qué fase entraría.
- `_conocimiento/` acumula lo que sale del método aplicado: insights
  de industria, casos, research reutilizable.

---

## 5. Lo que falta — y por qué es progresivo

### Fase actual (completada)
- Estructura de carpetas definida y migrada
- Rules operativas activas en `.claude/rules/`
- Inventario de automatizaciones con sync automático
- CLAUDE.md actualizado como mapa del sistema
- Brief de diseño para app UI generado

### Siguiente fase (por definir)
- Replicar estructura en Google Drive
- Mapear equivalencias estructura ↔ ClickUp
- Migrar contenido de carpetas legacy (Folder Gestion Dani, etc.)
- Poblar `_herramientas/templates/` con plantillas estandarizadas
- Definir cuáles dashboards se mantienen y cuáles se deprecan

### Fase de convergencia
- Recibir inputs de Luis sobre cómo él ve la organización
- Comparar su visión con esta estructura
- Hacer blend: lo que se mantiene, lo que se adapta, lo que se agrega
- Producir una estructura unificada que funcione en las 3 capas
  (local + Drive + ClickUp)

---

## 6. Para el blend con inputs de Luis

Este documento está diseñado para ser comparado lado a lado con los
inputs estratégicos de Luis Holder. El ejercicio de convergencia busca:

**Qué comparar:**
- ¿Su visión de carpetas/espacios coincide con esta estructura?
- ¿Qué categorías propone él que aquí no existen?
- ¿Qué nivel de detalle espera en ClickUp vs archivos?
- ¿Cómo ve la relación método ↔ clientes ↔ pipeline?

**Qué preservar de esta estructura:**
- El método como eje vertebral (no negociable)
- La secuencia 1→2→3→4 reflejada en carpetas
- El sistema de rules para configuración del AI
- El inventario de automatizaciones con changelog
- El mecanismo de triage (_inbox/)

**Qué es flexible:**
- Nombres de carpetas (se pueden ajustar a la nomenclatura de Luis)
- Nivel de profundidad en subcarpetas
- Qué contenido vive en archivos vs ClickUp
- Cómo se visualiza en la app

**Resultado esperado:**
Un documento unificado que sea la versión final de la estructura,
validado por ambas visiones, listo para implementar en las 3 capas.
