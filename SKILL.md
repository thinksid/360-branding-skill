---
name: 360-branding
description: >
  Use this skill whenever the user invokes /360-branding, or asks to apply 360xRunning brand guidelines,
  or wants to transform/convert/redesign/rebrand ANY asset (presentation, text, post, brief, PDF, outline,
  notes, or any other content) into a 360xRunning-branded piece. Also trigger when the user says things like
  "hazlo con la marca", "aplica el branding", "convierte esto a 360xrunning", "diseña esto para la marca",
  "con la identidad de 360", or any equivalent. The skill handles four output types: presentations (3 ambientes:
  charla/TED, para clientes, interna 360), social media (Instagram, TikTok, LinkedIn), invitaciones a eventos
  (webinars, encuentros, talleres, lanzamientos), web (HTML+CSS), and pautas/ads. Always use this skill when
  360xRunning brand alignment is involved — don't try to apply brand guidelines without consulting it.
---

# /360-branding — Skill de Identidad de Marca 360xRunning

Este skill transforma cualquier asset de entrada en un output 100% alineado con la identidad visual y de comunicación de 360xRunning.

## Paso 1: Entender el input y el output deseado

### Identificar el asset de entrada
El input puede ser cualquiera de los siguientes:
- Texto (notas, chat, outline, bullet points, script)
- Presentación existente (PPTX o Google Slides exportado)
- PDF con contenido
- Brief o descripción de lo que se quiere comunicar

### Preguntar por el output si no es explícito
Si el usuario no especifica claramente qué formato de salida quiere, **siempre pregunta** antes de continuar. Las opciones son:

1. **Presentación: Charla / TED** — Para eventos, conferencias, sponsors. Cinematográfica, la coach narra en vivo. **Siempre pregunta el objetivo de la charla** (inspirar a correr, posicionar la marca, storytelling de transformación, u otro) para definir el arco narrativo.
2. **Presentación: Para clientes** — La clienta consulta este contenido **sin coach presente**. Debe ser autocontenida: planes, reportes, guías educativas. La clienta entiende todo sola.
3. **Presentación: Interna 360** — Seguimiento, comités, sesiones de trabajo del equipo. Datos directos, estructura operativa, decisiones claras.
4. **Post de Instagram** — 1080×1080 px cuadrado
5. **Story/Reel de Instagram o TikTok** — 1080×1920 px vertical
6. **Post de LinkedIn** — 1200×627 px o 1080×1080 px
7. **Invitación a evento** — Digital (para WhatsApp, email, redes). Incluye QR de registro. Ver checklist de datos requeridos abajo.
8. **Página web / Landing page** — HTML + CSS
9. **Pauta publicitaria** — Especificar red y dimensiones

Ejemplo de pregunta al usuario:
> "¿Para qué formato quieres este contenido? ¿Presentación (charla/TED, para clientes, o interna 360)? ¿Post de Instagram, story, LinkedIn, invitación a evento, o página web?"

### Paso adicional para presentaciones tipo Charla / TED
Si el usuario elige **Charla / TED**, pregunta siempre por el **objetivo principal** antes de construir la narrativa:
> "¿Cuál es el objetivo principal de esta charla? ¿Inspirar a mujeres a correr, posicionar a 360xRunning como marca experta, compartir una historia de transformación, u otro?"

Este objetivo define el arco narrativo (ver `references/presentations.md`).

### Paso adicional para invitaciones a eventos
Si el usuario elige **Invitación a evento**, recoge los datos mediante un **checklist interactivo**. Pregunta uno por uno y confirma cada dato:

- [ ] **Tipo de evento**: Webinar/Live, Encuentro presencial, Taller/Workshop, o Evento de marca
- [ ] **Nombre del evento**
- [ ] **Fecha y hora**
- [ ] **Tema / descripción breve**
- [ ] **Coach o host** (nombre y rol)
- [ ] **Precio o "Gratis"**
- [ ] **Link de registro** (obligatorio — se genera QR automáticamente a partir de este link)
- [ ] **Lugar** (si es presencial) o **Plataforma** (si es virtual: Zoom, Instagram Live, etc.)
- [ ] **Dimensiones** deseadas (1080x1080 para feed, 1080x1920 para story, o ambas)

Solo procede a diseñar cuando el checklist esté completo.

---

## Paso 2: Cargar la referencia de marca correcta

**Lee siempre** `references/brand-identity.md` antes de diseñar cualquier output — contiene todos los valores exactos de colores, tipografía, tono de voz y reglas del logo.

Luego carga la referencia específica del formato:
- Presentación → `references/presentations.md`
- Invitación a evento → `references/invitations.md`
- Redes sociales → `references/social-media.md`
- Web → `references/web.md`

---

## Paso 3: Determinar la categoría del contenido

El contenido de 360xRunning se divide en tres categorías, cada una con su color primario:

| Categoría | Color primario | Uso |
|-----------|---------------|-----|
| **Entrenamiento** | Rosa `#F1ACA5` | Running, crosstraining, ejercicio, planes, suplementos |
| **Mente** | Terracota `#A8564D` | Mindfulness, metas, propósito, psicología deportiva |
| **Bienestar** | Verde `#163935` | Nutrición, hábitos, sueño, ciclo femenino, descanso |

Si el contenido es mixto o institucional (sobre la marca, equipo, patrocinadores), usa **Crema `#F1F1E8`** con acentos en Verde o Terracota.

---

## Paso 4: Producir el output

Sigue las instrucciones del archivo de referencia del formato correspondiente. Algunas reglas universales que aplican a TODOS los outputs:

### Reglas de identidad que nunca se rompen
1. **Solo colores de la paleta**: Rosa `#F1ACA5`, Crema `#F1F1E8`, Terracota `#A8564D`, Verde `#163935`. Nunca usar colores fuera de esta paleta.
2. **Solo Poppins**: Toda tipografía es de la familia Poppins. Nunca otra fuente.
3. **Logo**: Usar los archivos SVG de `assets/logos/` — elegir la variante correcta según el fondo (ver tabla en `references/brand-identity.md`). Respetar siempre el área de protección (2x en todos los lados).
4. **Tono siempre de "tú"**: Nunca "usted". El 99% del tiempo el mensaje va de mujer a mujer. 360xRunning es una figura de autoridad e inspiración para la mujer corredora.
5. **Idioma**: 90% español, 10% inglés (solo términos técnicos del running o fitness que se usan naturalmente en español, ej. "crosstraining", "split", "recovery").
6. **Fotografía**: Siempre de mujeres en contextos de running y bienestar femenino. Nunca imágenes genéricas o masculinas.

### Combinaciones de logo aprobadas
| Logo | Fondo |
|------|-------|
| Verde | Crema |
| Crema | Verde |
| Rosa | Terracota |
| Terracota | Rosa |
| Blanco | Cualquier color sólido oscuro (emergencias) |
| Negro | Blanco (solo impresión monocromática) |

---

## Paso 5: Entregar y verificar

Al entregar el output:
1. Menciona brevemente qué decisiones de marca tomaste (categoría elegida, combinación de colores, por qué).
2. Si faltan archivos del logo (se confirmarán cuando estén disponibles), indica dónde va posicionado y en qué variante.
3. Si el usuario no quedó satisfecho, pregunta específicamente qué cambiaría para iterar.
