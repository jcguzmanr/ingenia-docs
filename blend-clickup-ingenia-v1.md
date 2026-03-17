# ClickUp BLEND — Estructura Unificada Ingenia Latam (v1)
## Integración: Ingenia OS (JC) + Sistema Operativo Consultivo (Luis Holder)

**Fecha:** 17 de marzo de 2026
**Responsables:** JC (Director Operaciones Consultivas) + Luis Holder (CEO)
**Estado:** DRAFT v1 — Pendiente validación de links de Luis y decisiones de gobernanza
**Propósito:** Este documento propone la estructura unificada de ClickUp que integra la arquitectura de JC con la visión estratégica de Luis, mapeando equivalencias, proponiendo la estructura de 4 niveles, y un plan de implementación progresiva realista.

---

## ÍNDICE

1. Diagnóstico de convergencia
2. Estructura unificada propuesta para ClickUp
3. Los 7 procesos como Spaces (o Folders)
4. Plan de implantación progresiva (4 fases)
5. Qué falta resolver
6. Principios de diseño del blend

---

## 1. DIAGNÓSTICO DE CONVERGENCIA

### 1.1 Visión de JC — Ingenia OS

**Fuente:** `estructura-ingenia-os-v1.md`
**Enfoque:** Arquitectura de carpetas en 3 capas (Local + Drive + ClickUp)

**Estructura propuesta:**
```
🟠 Ingenia/
├── .claude/rules/              ← Configuración AI operativa
├── _método/fundacionales/      ← Fuente de verdad del modelo consultivo
├── _clientes/[cliente]/        ← Instancias vivas (1→2→3→4)
├── _pipeline/[prospecto]/      ← Prospectos pre-cliente
├── _operación/                 ← ClickUp, procesos, reportes, comités
├── _conocimiento/              ← IP acumulada
├── _herramientas/              ← Automatizaciones, skills, templates
└── _inbox/                     ← Triage
```

**Principios:**
- El método (1-negocio → 2-marca → 3-comunicación → 4-creatividad) es el eje vertebral
- Estructura espejo: cada cliente replica la secuencia de fases
- Pipeline conectado al método, no como proceso comercial puro
- Tres capas: archivos (qué se produjo), Drive (acceso compartido), ClickUp (quién hace qué cuándo)

**Lo que JC entrega en pipeline (ya avanzado):**
- 46 empresas en Excel, mapeadas
- 10 etapas del flujo de valor definidas
- 94 contactos extraídos
- AI Fields configurables con prompts claros
- Directorio de Contactos como lista separada
- Relaciones bidireccionales Pipeline ↔ Contactos

### 1.2 Visión de Luis — Sistema Operativo Consultivo

**Fuente:** Mensaje WhatsApp 15/03/26 + 12 links a ChatGPT
**Enfoque:** ClickUp como "cerebro estratégico" para gobernar 7 procesos del OS consultivo

**Temas cubiertos en los 12 links:**
1. Arquitectura ClickUp (lista por lista)
2. Sistema Operativo Consultivo (7 procesos, definidos pero no publicados aquí)
3. Workflows (1 workflow por proceso, con estados y checklists)
4. 7 Dashboards Estratégicos (1 por capa crítica del modelo consultivo)
5. Sistema de Comités Estratégicos (reemplazar WhatsApp/email)
6. Consultiva con IA (segunda capa de inteligencia estratégica)
7. Consulting Brain (memoria estratégica acumulativa)
8. Mapa completo del OS (pensar → decidir → ejecutar → aprender → mejorar)
9. Estructura exacta de ClickUp (4 niveles: Workspace → Spaces → Folders → Lists)
10. Plan de 7 días de implementación (instalar ritmo, no todo a la vez)
11. 10 Reglas de Oro (culturales, no técnicas: "la herramienta nunca falla; falla la disciplina")
12. Sistema de KPIs (medir si opera como consultora, no agencia)

**Frases clave de Luis:**
- "ClickUp refleje el pensamiento consultivo, no la producción de piezas"
- "Los 7 procesos del sistema operativo serán el esqueleto"
- "La disciplina semanal es lo que sostiene el modelo"
- "Pensar → decidir → ejecutar → aprender → mejorar"
- "Segunda capa de inteligencia estratégica" (AI)

---

### 1.3 Análisis de Convergencia

| Dimensión | JC | Luis | Convergencia |
|-----------|-----|------|--------------|
| **Eje articulador** | Método (1→2→3→4) | Modelo consultivo + 7 procesos OS | ✓ COMPATIBLE: El método es uno de los 7 procesos; los otros 6 son operacionales |
| **Estructura jerárquica** | 3 capas (archivos, Drive, ClickUp) | 4 niveles en ClickUp (WS→Space→Folder→List) | ✓ COMPATIBLE: Los 4 niveles de ClickUp son la capa de "ejecución"; archivos y Drive son "decisión y memoria" |
| **Pipeline** | 2 listas (Pipeline Empresas + Directorio Contactos), 10 etapas, AI Fields | Menciona "cuentas consultivas" pero no detalla estructura | ✓ COMPATIBLE: Lo que JC diseñó es la instancia del flujo de valor |
| **Gobernanza** | Comité estratégico con CLAUDE.md preparado | Comité estratégico con disciplina semanal | ✓ COMPATIBLE: JC tiene la metodología; Luis define la frecuencia y ritual |
| **Clientes** | Estructura de fases (_clientes/[cliente]/1-2-3-4/) | Menciona "gobierno de clientes" pero no estructura | ✓ PENDIENTE: Necesita definición en ClickUp cómo se refleja la estructura de fases |
| **AI integrada** | Mention en _herramientas/ pero no activa | "Consultiva con IA" como capa estratégica | ✓ PENDIENTE: Luis define los ámbitos; JC implementa config de prompts |
| **Ritmo operativo** | Hípotesis: diario + semanal + mensual | Plan de 7 días de implantación; "disciplina semanal" | ✓ COMPATIBLE: Necesita validación de rituales específicos |
| **KPIs / Medición** | No mencionado en estructura | Sistema de KPIs para medir si opera como consultora | ✓ PENDIENTE: Necesita definición; será dashboard en ClickUp |

**Conclusión:** Las dos visiones NO compiten. Son complementarias:
- **JC construye la estructura y la operación diaria** (archivos, carpetas, pipeline, AI Fields)
- **Luis define la gobernanza y la estrategia** (7 procesos, comités, dashboards, KPIs, disciplina)

El blend integrará ambas en una arquitectura única donde ClickUp sea el "orquestador" de los 7 procesos, reflejando el método consultivo en cada uno.

---

## 2. ESTRUCTURA UNIFICADA PROPUESTA PARA CLICKUP

### 2.1 Los 4 Niveles de ClickUp — Mapa General

```
Workspace: INGENIA LATAM
│
├─ Space 1: ESTRATEGIA (Pensar → Decidir)
│  ├─ Folder: Comités Estratégicos
│  │  └─ List: Sesiones de Comité + Acuerdos
│  ├─ Folder: Diagnosis & Research
│  │  └─ List: Proyectos de investigación estratégica
│  └─ Folder: Consulting Brain
│     └─ List: Hipótesis, frameworks, decisiones, aprendizajes acumulados
│
├─ Space 2: CONSULTIVA PIPELINE (Flujo de Valor)
│  ├─ Folder: Pipeline Consultivo
│  │  ├─ List: Pipeline de Empresas (46 + nuevos)
│  │  └─ List: Directorio de Contactos (94 + nuevos)
│  ├─ Folder: Licitaciones
│  │  └─ List: Licitaciones en curso
│  └─ Folder: SOWs & Propuestas
│     └─ List: Propuestas por enviar / en negociación
│
├─ Space 3: CLIENTES (Operación & Delivery)
│  └─ Folder: [Cliente A]
│     ├─ List: Fase 1 — Negocio
│     ├─ List: Fase 2 — Marca
│     ├─ List: Fase 3 — Comunicación
│     └─ List: Fase 4 — Creatividad
│  └─ Folder: [Cliente B]
│     ├─ List: Fase 1 — Negocio
│     └─ ... (idem)
│
├─ Space 4: OPERACIÓN INTERNA (Ejecutar → Aprender)
│  ├─ Folder: Tareas operacionales
│  │  └─ List: Tareas de equipo (sincronía diaria/semanal)
│  ├─ Folder: Reuniones & Rituales
│  │  └─ List: Calendario de eventos (status diarios, semanales, comités)
│  └─ Folder: KPIs & Reportería
│     └─ List: Indicadores consultivos, dashboard de ejecución
│
└─ Space 5: CONOCIMIENTO (Aprender → Mejorar)
   ├─ Folder: Research acumulado
   │  └─ List: Industrias, verticales, insights
   ├─ Folder: Casos y referencias
   │  └─ List: Casos cerrados, learnings, benchmarks
   └─ Folder: Plantillas & Procesos
      └─ List: Templates de propuestas, briefs, documentos
```

---

### 2.2 Estructura Detallada por Space

#### **SPACE 1: ESTRATEGIA (Pensar → Decidir)**

**Propósito:** Gobernanza estratégica, decisiones de dirección, accumulation de conocimiento.

**Folder 1.1 — Comités Estratégicos**

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | [Fecha] — [Tipo]: Pipeline / Clientes / Licitaciones / General |
| Tipo de Comité | Dropdown | Pipeline · Clientes · Licitaciones · General · Estratégico |
| Fecha de sesión | Date | Cuándo fue/será el comité |
| Responsable | People | Luis o director que lidera |
| Estado | Status | Preparación · En curso · Completado · Pendiente acuerdos |
| Acuerdos | Long Text | Decisiones formales tomadas en la sesión |
| Asistentes | People (Multi) | Quién participó |
| Attachments | Files | Link a registro, audio, acta |

**Folder 1.2 — Diagnosis & Research**

Proyectos de investigación estratégica que informan decisiones de negocio o pipeline.

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Nombre del proyecto de research |
| Tipo | Dropdown | Industria · Vertical · Competencia · Mercado · Interno |
| Estado | Status | Iniciado · En desarrollo · Completado · Archivado |
| Responsable | People | Quién lidera |
| Insights clave | Long Text | Hallazgos principales |
| Aplicación | Text | A qué decisión/prospecto aplica |
| Fecha de inicio | Date | Cuándo se inició |
| Fecha de entrega | Date | Cuándo se completó |

**Folder 1.3 — Consulting Brain**

Sistema vivo de memoria estratégica: hipótesis, frameworks, decisiones y aprendizajes acumulados. (Este concepto es de Luis; está por definir contenido)

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Titulo del insight/hipótesis/framework/decisión |
| Tipo | Dropdown | Hipótesis · Framework · Decisión · Aprendizaje · Patrón |
| Fecha de registro | Date | Cuándo se capturó |
| Contexto | Long Text | De dónde surge (prospecto, cliente, investigación) |
| Contenido | Long Text | La hipótesis/framework/decision en sí |
| Relevancia | Dropdown | Alta · Media · Baja |
| Vinculado a (Relación) | Task Link | Prospectos/clientes donde aplica |

---

#### **SPACE 2: CONSULTIVA PIPELINE (Flujo de Valor)**

Aquí vive el pipeline que JC ya diseñó, más las licitaciones y propuestas.

**Folder 2.1 — Pipeline Consultivo**

**List 2.1.1 — Pipeline de Empresas**

(Estructura ya detallada en `Pipeline_ClickUp_Rediseño_Columnas.md`)

| Sección | Campos |
|---------|--------|
| **Base** | Empresa, Sector, Tipo de Prospecto, Canal entrada, Fecha inicio |
| **Inteligencia** | Tensión Detectada, Hipótesis Estratégica, [AI] Calidad tensión, [AI] Fortaleza hipótesis |
| **Pipeline** | Etapa (Status), Días en etapa (Formula), Valor fee (Currency), Probabilidad (%), [AI] Urgencia |
| **Operativo** | Última interacción, [AI] Resumen interacción, Próximo paso, [AI] Urgencia del paso, Responsable |
| **Gobernanza** | Decisión comité, [AI] Recomendación decisión, Fecha última revisión, Fecha próxima revisión, Semáforo, Acuerdo revisión, [AI] Narrative brief, Observaciones |

**Status de Pipeline (10 etapas + 3 finales):**
```
Pre-pipeline (Backlog):
  → Sin contactar

Activo:
  → Selección estratégica (Etapa 1)
  → Registrado en pipeline (Etapa 2)
  → Primera reunión estratégica (Etapa 3)
  → Hipótesis de valor (Etapa 4)
  → Definición de alcance (Etapa 5)
  → Gobernanza interna (Etapa 6)

Negociación:
  → Propuesta enviada (Etapa 7)
  → En negociación (Etapa 8)
  → Cierre (Etapa 9)

Cerrado:
  → Transferido a operación (Cerrado-Ganado)
  → Descartado (Cerrado-Perdido)
  → En pausa (Inactivo)
```

**List 2.1.2 — Directorio de Contactos**

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Nombre completo | Task Name | Nombre de la persona |
| Empresa | Relationship | Vinculo a Pipeline de Empresas |
| Cargo / Rol | Text | CMO, CIO, Gerente, etc. |
| Email | Email | Dato de contacto |
| Teléfono | Phone | Dato de contacto |
| Nivel de Poder | Dropdown | Alto · Medio · Bajo |
| Tipo de interlocutor | Dropdown | Decisor · Influenciador · Operativo · Gatekeeper |
| Canal preferido | Dropdown | Email · WhatsApp · LinkedIn · Llamada |
| Estado | Dropdown | Activo · Inactivo · Sin respuesta · Convertido a cliente |
| Última interacción | Date | Cuándo fue el último contacto |
| Notas | Long Text | Contexto, relación, preferencias |

---

**Folder 2.2 — Licitaciones**

Cuando un prospecto entra en etapa de licitación formal, se abre una tarea aquí con toda la documentación de ese proceso.

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | [Empresa] — Licitación [Código/Fecha] |
| Empresa | Relationship | Vinculo a Pipeline de Empresas |
| Fecha de publicación | Date | Cuándo se abre la licitación |
| Fecha de cierre | Date | Deadline para enviar propuesta |
| Presupuesto estimado | Currency | Si está publicado |
| Alcance licitado | Long Text | Qué pide |
| Estado | Status | Abierta · Propuesta en desarrollo · Propuesta enviada · Resultado pendiente · Ganada · Perdida |
| Responsable | People | Quién lidera la propuesta |
| Equipo asignado | People (Multi) | Quiénes participan |
| Documentos | Files | Bases, brief interno, propuesta borrador, propuesta final |
| [AI] Análisis de encaje | AI Field | ¿Esta licitación encaja con el modelo consultivo? |
| Notas | Long Text | Observaciones |

---

**Folder 2.3 — SOWs & Propuestas**

Todas las propuestas que estamos desarrollando o hemos enviado (incluyendo propuestas comerciales que no sean licitación formal).

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | [Empresa] — Propuesta [Fecha] |
| Empresa | Relationship | Vinculo a Pipeline |
| Fecha de creación | Date | Cuándo se inició la propuesta |
| Fecha de envío | Date | Cuándo se envió (si aplica) |
| Tipo de propuesta | Dropdown | SOW · Pitch · Brief · Propuesta comercial |
| Responsable | People | Quién la redacta |
| Estado | Status | Borrador · En revisión · Lista para enviar · Enviada · Aceptada · Rechazada |
| Fee propuesto | Currency | Valor del proyecto |
| Alcance | Long Text | Qué se propone |
| Versiones | Files | v1, v2, final, pdf |
| Feedback | Long Text | Comentarios del cliente |

---

#### **SPACE 3: CLIENTES (Operación & Delivery)**

Refleja la estructura de carpetas que JC propuso: cada cliente tiene sus 4 fases del método.

```
SPACE: CLIENTES

Folder: [Cliente A] — Nicovita / Vitapro
  ├─ List: Fase 1 — Negocio (si hay contenido)
  ├─ List: Fase 2 — Marca (si hay contenido)
  ├─ List: Fase 3 — Comunicación (si hay contenido)
  └─ List: Fase 4 — Creatividad (si hay contenido)

Folder: [Cliente B] — [Nuevo]
  ├─ List: Fase 1 — Negocio
  └─ (idem)
```

**Estructura de cada List (Fase)**

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Nombre del entregable o workstream |
| Fase | Label | Automático según la List |
| Cliente | Dropdown | Qué cliente |
| Tipo de entregable | Dropdown | Análisis · Documento · Presentación · Recomendación · Otro |
| Estado | Status | Backlog · En desarrollo · En revisión · Completado · Entregado |
| Responsable | People | Quién ejecuta |
| Revisor | People | Quién valida antes de cliente |
| Fecha de inicio | Date | Cuándo comienza |
| Fecha de entrega | Date | Cuándo se debe entregar |
| Descripción | Long Text | Qué es el entregable |
| Documentos | Files | Borrador, versiones, entrega final |
| Horas estimadas | Number | Para control de rentabilidad |
| Horas reales | Number | Para tracking |

---

#### **SPACE 4: OPERACIÓN INTERNA (Ejecutar → Aprender)**

Tareas operacionales, rituales y reportería.

**Folder 4.1 — Tareas Operacionales**

Donde viven las tareas diarias de equipo (no vinculadas a un cliente o prospecto específico).

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Descripción de la tarea |
| Tipo | Dropdown | Admin · Proceso · Mejora · Investigación |
| Asignado a | People | Responsable |
| Fechavencimiento | Date | Cuándo debe estar lista |
| Prioridad | Dropdown | Crítica · Alta · Normal · Baja |
| Estado | Status | Backlog · En desarrollo · En revisión · Completado |

---

**Folder 4.2 — Reuniones & Rituales**

Registro de eventos clave (status diarios, semanales, comités, etc.).

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | [Tipo] — [Fecha] |
| Tipo de reunión | Dropdown | Status diario · Status semanal · Comité · Retrospectiva · Otra |
| Fecha | Date | Cuándo es/fue |
| Hora | Time | Hora de inicio |
| Responsable | People | Quién lidera |
| Asistentes | People (Multi) | Quiénes asisten |
| Orden del día | Long Text | Temas a tratar |
| Notas | Long Text | Lo que se discutió |
| Decisiones | Long Text | Qué se acordó |
| Attachment | Files | Recording, acta, etc. |

---

**Folder 4.3 — KPIs & Reportería**

Tracking de indicadores consultivos. (A definir con Luis qué KPIs se miden)

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | [KPI] — [Período] |
| KPI | Dropdown | (A definir según sistema de KPIs de Luis) |
| Período | Dropdown | Semanal · Mensual · Trimestral |
| Valor meta | Number | Qué se espera |
| Valor real | Number | Qué se logró |
| Estado | Status | En tracking · Completado |
| Análisis | Long Text | Interpretación del número |

---

#### **SPACE 5: CONOCIMIENTO (Aprender → Mejorar)**

Documentación, research y aprendizajes acumulados.

**Folder 5.1 — Research Acumulado**

Estudios de industria, verticales, tendencias, mercados que informan la estrategia de pipeline o clientes.

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Tema del research |
| Tipo | Dropdown | Industria · Vertical · Tendencia · Mercado · Benchmark |
| Resumen | Long Text | Hallazgos principales |
| Aplicación | Text | A qué se aplica |
| Documento | Files | Link o documento adjunto |
| Fecha | Date | Cuándo se realizó |

---

**Folder 5.2 — Casos y Referencias**

Casos cerrados, learnings, referencias que son IP de Ingenia.

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Nombre del caso / learning |
| Tipo | Dropdown | Caso ganado · Caso perdido · Learning interno · Best practice |
| Descripción | Long Text | Qué pasó, qué aprendimos |
| Aplicable a | Text | Qué verticales, qué tipo de prospectos |
| Documentos | Files | Materiales, documentación |
| Fecha | Date | Cuándo ocurrió |

---

**Folder 5.3 — Plantillas & Procesos**

Templates reutilizables: propuestas, briefs, documentos, procesos operativos.

| Campo | Tipo | Descripción |
|-------|------|-------------|
| Task Name | Text | Nombre de la plantilla |
| Tipo | Dropdown | Propuesta · Brief · Contrato · Proceso · Presentación · Otro |
| Descripción | Text | Para qué se usa |
| Documento | Files | Archivo template |
| Última actualización | Date | Cuándo se actualizó |
| Responsable | People | Quién mantiene la plantilla |

---

### 2.3 Vistas Clave por Space

Cada Space/List debe tener múltiples vistas (Kanban, Table, Calendar, etc.) para diferentes formas de trabajo.

**Space 1 — ESTRATEGIA:**
- Table: Comités (cronológico, con decisiones)
- Calendar: Próximos comités (visualizar frecuencia)

**Space 2 — PIPELINE:**
- Kanban: Pipeline de Empresas (por Status/Etapa) — vista principal
- Table: Pipeline de Empresas (data completa, para comité)
- Table: Directorio de Contactos (para exportar mails)
- Calendar: Licitaciones (deadline de licitaciones)

**Space 3 — CLIENTES:**
- Table: Entregables por cliente (para proyecto manager de cada cliente)
- Calendar: Fechas de entrega (para visión ejecutiva)

**Space 4 — OPERACIÓN:**
- Table: Tareas (filtradas por asignado, prioridad, estado)
- Calendar: Reuniones (sincronización visual del equipo)

**Space 5 — CONOCIMIENTO:**
- Table: Catálogo de research, casos, plantillas

---

## 3. LOS 7 PROCESOS COMO SPACES (O FOLDERS)

### Inferencia basada en contexto

Luis menciona "7 procesos del sistema operativo" pero no publica el contenido en el mensaje WhatsApp. Sin embargo, del contexto de su mensaje y del método consultivo, podemos inferir cuáles serían:

| Proceso | Descripción | Instancia en ClickUp | Dueño |
|---------|-------------|----------------------|-------|
| **1. Pensamiento Estratégico** | Investigación, diagnóstico, generación de hipótesis | Space: ESTRATEGIA (Diagnosis & Research) | Rodrigo (Dir. Estrategia) |
| **2. Prospección Consultiva** | Identificación, cualificación, primera reunión con prospectos | Space: PIPELINE (Pipeline de Empresas, etapas 0-5) | Luis + equipo |
| **3. Propuesta Consultiva** | Desarrollo, gobernanza, envío de propuestas | Space: PIPELINE (SOWs & Propuestas, licitaciones) | Rodrigo + JC |
| **4. Gobierno de Clientes** | Gestión de fases del método, entregas, relación con cliente | Space: CLIENTES (Fases 1-4) | JC + equipo de cuenta |
| **5. Ejecución Operativa** | Tareas diarias, rituales, sincronización del equipo | Space: OPERACIÓN | Todos |
| **6. Gobernanza & Decisiones** | Comités, acuerdos, decisiones estratégicas | Space: ESTRATEGIA (Comités) | Luis + directores |
| **7. Aprendizaje & Mejora** | Captura de knowledge, consultoría interna, mejora continua | Space: CONOCIMIENTO (Research, casos, brain) | Todos + curador central |

**Nota:** Esta es una inferencia. Luis debe validar:
- ¿Son estos los 7 procesos?
- ¿Hay otros?
- ¿Cómo se relacionan con los que menciona en sus links?

---

## 4. PLAN DE IMPLANTACIÓN PROGRESIVA (4 FASES)

El plan de 7 días de Luis es ambicioso. Aquí proponemos una versión realista que avanza en paralelo sin sobrecargar.

### 4.1 FASE 0 — Foundation (Completada / En curso)

**Qué está hecho:** Estructura local, rules operativas, Ingenia OS, Pipeline rediseño en Excel.

| Tarea | Estado | Responsable |
|-------|--------|-------------|
| Estructura Ingenia OS local | ✓ Completado | JC |
| Rules de AI operativas | ✓ Completado | JC |
| Análisis Pipeline_ClickUp (rediseño columnas) | ✓ Completado | JC |
| Análisis datos 46 empresas | ✓ Completado | JC |
| Definición AI Fields + prompts | ✓ Completado | JC |
| Comité estratégico (metodología CLAUDE.md) | ✓ Completado | JC |

**Dependencias para avanzar:**
- Validación de Luis sobre 7 procesos
- Acceso ClickUp con espacios disponibles

**Fecha target:** 17/03/26 (hoy)

---

### 4.2 FASE 1 — Core Structures (1.5 semanas)

**Objetivo:** Montar la estructura base en ClickUp, comenzar a operar.

**Semana 1 (17-21 marzo):**

1. **Crear Workspaces y Spaces en ClickUp**
   - Workspace: INGENIA LATAM
   - Space 1: ESTRATEGIA
   - Space 2: PIPELINE
   - Space 3: CLIENTES (con Nicovita como pilot)
   - Space 4: OPERACIÓN
   - Space 5: CONOCIMIENTO
   - **Responsable:** JC + Mercedes (si tiene acceso ClickUp)
   - **Duración:** 2 horas
   - **Bloqueante:** Acceso ClickUp

2. **Crear Lists y Custom Fields base (Phase 1 del plan de JC)**
   - Folder ESTRATEGIA > List Comités
   - Folder PIPELINE > List Pipeline de Empresas (con 13 Statuses, campos base)
   - Folder PIPELINE > List Directorio de Contactos
   - Folder CLIENTES/Nicovita > Lists Fase 1-4
   - Folder OPERACIÓN > List Tareas operacionales
   - **Responsable:** JC + ClickUp admin
   - **Duración:** 4 horas (configuración manual UI)
   - **Nota:** Los Custom Fields (dropdowns, fórmulas, Relationship) se crean en UI

3. **Comenzar migración de datos (Phase 2 del plan de JC)**
   - Migrar las 46 empresas del Excel a ClickUp (como tareas en Pipeline)
   - Crear los 94 contactos como tareas en Directorio
   - Vincular contactos ↔ empresas (Relationship field)
   - **Responsable:** Claude vía MCP (bulk create tasks)
   - **Duración:** 3 horas scripting + validación manual
   - **Tools disponibles:** `clickup_create_task`, `clickup_update_task`

4. **Activar ritmo operativo**
   - Primer comité en ClickUp (17/03 o 18/03)
   - Registrar en List de Comités
   - **Responsable:** JC + Luis
   - **Duración:** 1.5 horas

**Semana 2 (24-28 marzo):**

5. **Configurar AI Fields (Phase 3 del plan de JC)**
   - En ClickUp UI: activar 5 AI Fields del pipeline con prompts de JC
   - Validar outputs con 10 empresas pilot
   - **Responsable:** JC + ClickUp admin
   - **Duración:** 3 horas

6. **Crear vistas Kanban**
   - Vista Kanban del Pipeline (por Status)
   - Hacer visible a todo el equipo
   - **Responsable:** JC
   - **Duración:** 1 hora

7. **Checkpoint: Validación de Luis**
   - ¿Se ve el pensamiento consultivo?
   - ¿Faltan procesos o campos?
   - Feedback para ajustes
   - **Reunión:** 24 o 25 marzo

**Criterios de éxito de Phase 1:**
- Los 46 prospectos están en ClickUp
- El pipeline es visible en Kanban
- El equipo puede abrir ClickUp y ver dónde están las cosas
- Primer comité registrado en ClickUp

---

### 4.3 FASE 2 — Clientes & Gobernanza (2-3 semanas)

**Objetivo:** Operación en clientes activos, comités recurrentes, dashboards básicos.

**Actividades:**

1. **Estruturar clientes existentes en ClickUp**
   - Migrar Nicovita: definir dónde están actualmente (fase 1, 2, 3, 4?)
   - Crear Lists para cada fase
   - Migrar entregables de archivo a ClickUp
   - **Responsable:** JC
   - **Duración:** 4 horas

2. **Automatizaciones básicas del pipeline**
   - Alertas: Días en etapa > 30 → Semáforo amarillo
   - Alertas: Días en etapa > 60 → Semáforo rojo
   - Reminder: Próxima revisión vencida
   - **Responsable:** ClickUp admin / Claude (Automations)
   - **Duración:** 2 horas

3. **Comités recurrentes**
   - Establecer cadencia: Pipeline (quincenalmente), Clientes (mensual), Estratégico (semanal)
   - Registrar en Calendar + Ritual List
   - Preparar template de agenda
   - **Responsable:** JC + Luis
   - **Duración:** 2 horas

4. **Dashboards iniciales** (3 dashboards de los 7 que Luis propone)
   - Dashboard 1: Pipeline health (estados, días, semáforos)
   - Dashboard 2: Clientes activos (fases, entregables, timeline)
   - Dashboard 3: Reuniones & ritual (próximas sesiones)
   - **Responsable:** JC + ClickUp admin
   - **Duración:** 6 horas

**Criterios de éxito:**
- Clientes operando en ClickUp (al menos 1 piloto)
- Comités recurrentes en sistema
- Dashboards básicos visibles a directores
- Alertas automáticas funcionando

---

### 4.4 FASE 3 — AI Integration & Consulting Brain (3-4 semanas)

**Objetivo:** Segunda capa de inteligencia estratégica; memory system.

**Actividades:**

1. **Consultoría AI integrada**
   - Evaluar dónde meter Prompts de AI en ClickUp
   - Configurar AI Fields adicionales (más allá de los 5 del pipeline)
   - Testing con casos reales
   - **Responsable:** JC + Claude
   - **Duración:** 4 horas

2. **Consulting Brain structure**
   - Definir qué va en Space CONOCIMIENTO
   - Crear List: Hipótesis
   - Crear List: Frameworks
   - Crear List: Decisiones
   - Crear List: Learnings
   - Poplar con datos iniciales de Nicovita y propuestas
   - **Responsable:** JC + Rodrigo
   - **Duración:** 5 horas

3. **Dashboards estratégicos (4 más de los 7)**
   - Dashboard KPIs (si Luis define qué medir)
   - Dashboard Consulting Brain (hipótesis activas, patterns)
   - Dashboard Revenue Pipeline (fee estimado, probabilidad, ARR)
   - Dashboard Ritual (comités, decisiones, acuerdos)
   - **Responsable:** JC + ClickUp admin
   - **Duración:** 8 horas

4. **Evaluación y ajuste**
   - Feedback de equipo en 1:1 + grupo
   - Qué está funcionando, qué no
   - Correcciones antes de "go live"
   - **Responsable:** JC + Luis
   - **Duración:** 3 horas

**Criterios de éxito:**
- AI Fields generando insights útiles
- Consulting Brain capturando hipótesis y learnings reales
- 6-7 dashboards estratégicos listos
- Equipo viendo valor diferencial vs. WhatsApp/email

---

### 4.5 FASE 4 — Scale & Operationalize (Ongoing)

**Objetivo:** Consolidar como sistema operativo oficial.

**Actividades:**

1. **Migración de otros clientes**
   - Trasladar en carpetas de ClickUp estructura de fases
   - Crear ritmos de comité por cliente
   - **Responsable:** JC
   - **Duración:** 1 hora por cliente (después del primero)

2. **Adoptación del equipo**
   - Entrenamientos en ClickUp (no es manual, es hands-on)
   - Crear cultura de ritual (comité = norma, no excepción)
   - KPIs: % uso ClickUp vs. WhatsApp para decisiones
   - **Responsable:** JC + Rodrigo
   - **Duración:** Ongoing

3. **Sync with Drive & Archivos**
   - Google Drive replica estructura de ClickUp (carpetas espejo)
   - Vincular referencias entre archivo local y ClickUp
   - **Responsable:** JC + DevOps
   - **Duración:** 2 horas setup, luego automatizado

4. **Mejora continua**
   - Retrospectiva mensual: qué trabajó, qué ajustar
   - Feedback loop: equipo → JC → Luis → ajustes
   - Evolución de prompts de AI según aprendizaje
   - **Responsable:** JC
   - **Duración:** 1 hora mensual

---

### 4.6 Timeline General

```
Semana 1 (17-21 mar):    Phase 1A — Core structures (Workspace, Spaces, Lists, migración básica)
Semana 2 (24-28 mar):    Phase 1B — AI Fields, vistas, checkpoint con Luis
Semana 3-4 (31-11 abr):  Phase 2 — Clientes, comités, dashboards iniciales
Semana 5-7 (14-25 abr):  Phase 3 — AI integration, Consulting Brain, dashboards full
Semana 8+:               Phase 4 — Scale, adopción, mejora continua

Total: ~10 semanas para full operationalization (vs. 7 días del plan de Luis)
Ritmo: Incremental, no big bang. Equipo usando ClickUp desde semana 2.
```

---

## 5. QUÉ FALTA RESOLVER

### 5.1 De los links de Luis (por validar)

| Pregunta | Por qué importa | Owner |
|----------|-----------------|-------|
| ¿Cuáles son exactamente los 7 procesos? | Necesitamos mapeo 1:1 a Spaces/Folders de ClickUp | Luis |
| ¿Cuál es el detalle de cada workflow (estados, checklist, responsables)? | Definirá la estructura exacta de cada List | Luis |
| ¿Cuáles son los 7 dashboards estratégicos? ¿Qué métricas cada uno? | Necesario para Phase 3 | Luis |
| ¿Cuál es el sistema de KPIs completo? | Para medir si operamos como consultora | Luis |
| ¿Cuál es el contenido de "Consulting Brain" con ejemplos? | Para saber qué estructurar | Luis |
| ¿Las 10 Reglas de Oro? | Contexto cultural para implementación | Luis |
| ¿Plan de 7 días con secuencia exacta? | Para validar si nuestro timeline es realista | Luis |

**Recomendación:** JC + Luis deberían hacer una sesión de 2 horas para recorrer los 12 links y destilando:
1. Estructura exacta de Workspace
2. 7 procesos definitivos
3. KPIs a medir
4. Reglas de oro
5. Plan de implantación validado

---

### 5.2 Decisiones internas (por JC + Luis)

| Decisión | Opciones | Impacto | Owner |
|----------|----------|---------|-------|
| ¿Retirar o duplicar en Drive? | Replicar estructura en Drive + vinculación; o mantener solo ClickUp como fuente | Si Drive, requiere sync automática | JC + Devops |
| ¿Quién es admin de ClickUp? | JC, Mercedes, otro | Influye en velocidad de configuración | Luis |
| ¿Acceso de clientes (guests)? | Solo visibilidad de su cuenta; o acceso limitado a comités | Definirá Space 3 y Folder 4.2 | Luis |
| ¿Usar nativamente AI Fields o scripts externos? | ClickUp native tiene límites; scripts pueden ser más poderosos | Costo-beneficio API vs. UI | JC |
| ¿Cuándo comenzar full operación? | Semana 2 (riesgo: incompleto) vs. Semana 4 (conservador) | Adopción de equipo | Luis + JC |
| ¿Quién es el "curador" del Consulting Brain? | JC, Rodrigo, otro | Requiere disciplina semanal | Luis |

---

### 5.3 Contenido a criar/poblar

| Ítem | Dónde | Quién | Cuándo |
|------|-------|-------|--------|
| Definiciones finales de los 7 procesos | CLAUDE.md o doc referencia | Luis | Antes de Phase 1B |
| Plantillas operativas (propuesta, brief, SOW) | Space 5 / Folder Templates | Rodrigo + equipo | Phase 2 |
| Primeros learnings del Consulting Brain (de Nicovita) | Space 1 / Consulting Brain | JC + Rodrigo | Phase 3 |
| Casos cerrados + references | Space 5 / Casos y referencias | Todos | Ongoing |
| Research de industria foundacional | Space 5 / Research | Rodrigo | Phase 2 |
| KPIs iniciales + baseline | Space 4 / KPIs | JC + Luis | Phase 2 |

---

## 6. PRINCIPIOS DE DISEÑO DEL BLEND

Estos principios guiaron la integración y deben guiar la implementación:

### 6.1 El Método es el Eje (No Negociable)

La secuencia 1-negocio → 2-marca → 3-comunicación → 4-creatividad se refleja en:
- Estructura de carpetas de clientes (Space 3)
- Etapas del pipeline (Space 2)
- Modelo de valor de propuestas
- Frameworks de estrategia (Space 1)

**Implicancia:** Ninguna propuesta, cliente o prospecto se opera fuera de este eje. Si una oportunidad no encaja, se descarta.

---

### 6.2 ClickUp es el Orquestador, No el Repositorio

ClickUp refleja **quién hace qué, cuándo, en qué estado**. Los archivos (locales y Drive) contienen **qué se produjo y el conocimiento**.

- ClickUp = tasks, estados, responsables, fechas, decisiones
- Archivos = análisis, documentos, templates, research, IP

**Implicancia:** No duplicar contenido. Si algo se genera en un documento análisis, va al archivo; en ClickUp solo su metadata y task wrapper.

---

### 6.3 Los 7 Procesos son el Esqueleto

Cada proceso tiene su propio Space (o Folder en ESTRATEGIA si aplica), con:
- Listas de tareas/status
- Workflows definidos
- Responsables claros
- Ritmo de gobernanza

**Implicancia:** Si algo no encaja en los 7 procesos, probablemente es trabajo operativo menor (Space 4) o triage (no debe estar en ClickUp).

---

### 6.4 Disciplina Semanal > Automación

Las herramientas nunca salvan desorganización. El éxito depende de:
- Comités en ritmo (semanal/quincenal/mensual, no esporádico)
- Registros completos (no data incompleta que hace que AI Fields fallen)
- Decisiones formales documentadas
- Responsables identificados

**Implicancia:** ClickUp es un espejo de la disciplina. Si no hay disciplina, ClickUp expone el caos.

---

### 6.5 AI como Segunda Capa de Inteligencia, No Reemplazo

Los AI Fields sugieren, evalúan, resumen. Pero las decisiones reales las toma el equipo en comité.

**Ejemplos:**
- AI sugiere "Descartar" un prospecto → comité decide
- AI genera "narrative brief" para sesión → comité lo discute
- AI clasifica "tensión como táctica" → equipo valida

**Implicancia:** Los prompts deben ser claros pero no determinísticos. El AI Field es una herramienta de análisis, no un oráculo.

---

### 6.6 Progresivo, No Big Bang

Mejor comenzar con 60% funcional operando que 100% planeado sin usar.

- Phase 1: Pipeline operando (2 semanas)
- Phase 2: Clientes + comités operando (3 semanas adicionales)
- Phase 3: AI + Brain funcionando (3 semanas más)

Cada fase validada antes de escalar.

**Implicancia:** El plan de 7 días de Luis es la aspiración. La realidad es 10 semanas de adopción progresiva.

---

### 6.7 Reflejar el Pensamiento Consultivo, No la Ejecución Táctica

ClickUp debe dar respuesta a preguntas de nivel CEO/Estrategia, no de gestor operativo:
- ¿A dónde va el pipeline?
- ¿En qué fase está cada cliente?
- ¿Cuáles son las hipótesis que hemos desarrollado?
- ¿Qué hemos aprendido?
- ¿Qué decisiones se tomaron y por qué?

**No debe responder:**
- ¿Quién termina el informe de 50 páginas hoy?
- ¿Cuántas piezas creativas se hicieron?
- ¿Cuántos emails se mandaron?

**Implicancia:** Algunos espacios/lists pueden parecer "vacíos" porque no hacemos work production tracking. Eso es intencional.

---

## ANEXO A — Mapeo Preliminar de los 7 Procesos a ClickUp

(Sin validación de Luis; será ajustado cuando comparta los links)

| Proceso | Space(s) | Folder(s) | List(s) | Owner propuesto |
|---------|----------|-----------|---------|-----------------|
| 1. Pensamiento Estratégico | ESTRATEGIA | Diagnosis & Research | Proyectos de research | Rodrigo |
| 2. Prospección Consultiva | PIPELINE | Pipeline Consultivo | Pipeline de Empresas (etapas 0-5) | Luis + JC |
| 3. Propuesta Consultiva | PIPELINE | SOWs & Propuestas, Licitaciones | Propuestas, Licitaciones | Rodrigo |
| 4. Gobierno de Clientes | CLIENTES | [Cliente X] | Fases 1-4 | JC |
| 5. Ejecución Operativa | OPERACIÓN | Tareas Operacionales | Tareas | Todos |
| 6. Gobernanza & Decisiones | ESTRATEGIA | Comités Estratégicos | Sesiones de Comité | Luis |
| 7. Aprendizaje & Mejora | CONOCIMIENTO + ESTRATEGIA | Research + Consulting Brain | Todos | JC (curador) |

---

## ANEXO B — Template de ClickUp Task para Propuesta Consultiva (Ejemplo Oka)

```
Task Name:       Oka — Propuesta Consultiva (Marca en punto de venta)
Empresa:         Oka (Relationship → Pipeline de Empresas)
Tipo:            Propuesta Consultiva
Fase:            Gobernanza interna (etapa 6 del pipeline)

Responsable:     Rodrigo
Revisor:         Luis

Tensión:         Construcción de rol de marca previo al punto de venta
                 para mejorar conversión en tienda.

Hipótesis:       Si Oka entra antes en la decisión de marca, sube
                 conversión en tienda.

Alcance propuesto:
  1. Diagnóstico de marca actual + insights de tienda (Fase 1)
  2. Estrategia de marca para tienda (Fase 2)
  3. Activos comunicacionales (Fase 3)

Fee propuesto:   $XX,XXX

Status:          En gobernanza interna

Equipo:          Rodrigo (Lead), [Designers], [Community], [Data]

Riesgos:         ¿El fee cubre la profundidad de las 3 fases?
                 ¿El equipo tiene capacity?

Próximo paso:    Cierre de gobernanza interna + validación de fee
Fecha:           21 de marzo

Attachments:     - SOW borrador v1
                 - Hallazgos de Studio A (pending)
                 - Brief interno consultivo
```

---

## CONCLUSIÓN

Este documento propone una arquitectura unificada de ClickUp que:

1. **Preserva la visión de JC** sobre el método como eje, la estructura de carpetas, y la operación en 3 capas.

2. **Integra la estrategia de Luis** sobre los 7 procesos, el pensamiento consultivo, la disciplina semanal y los dashboards de gobernanza.

3. **Propone un plan realista** que es progresivo, basado en Phase gates de validación, no en un big bang de 7 días.

4. **Identifica claramente qué falta** por parte de Luis (contenido de los 12 links) y qué decisiones debe tomar el equipo.

5. **Usa terminología correcta de ClickUp** (Workspace, Spaces, Folders, Lists, Status, Custom Fields, AI Fields, Views).

**Próximos pasos:**
- Validación de este BLEND con Luis (1 sesión de 2h)
- Recorrer los 12 links + destilación
- Refinement de la estructura de Spaces
- Inicio de Phase 1 (semana de 17 marzo)

---

*Documento preparado por: JC (Claude Code)
Fecha: 17 de marzo de 2026
Versión: DRAFT v1
Validación pendiente: Luis Holder (7 procesos, KPIs, dashboards, plan 7d)*
