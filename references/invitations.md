# 360xRunning — Invitations Reference

> Loaded by /360-branding when the output is an event invitation.

## Formato

Solo digital. Las invitaciones se distribuyen por WhatsApp, email e Instagram (feed o stories).

## Dimensiones

| Canal principal | Dimensiones | Uso |
|----------------|-------------|-----|
| Feed Instagram / WhatsApp | 1080×1080 px | Cuadrado, versatil para ambas plataformas |
| Story Instagram / WhatsApp Status | 1080×1920 px | Vertical, para stories y estados |

Si el usuario no especifica, producir **ambas versiones** (cuadrada + vertical).

## Tipos de evento

| Tipo | Ejemplos | Tono visual |
|------|----------|-------------|
| **Webinar / Live** | Instagram Live, Zoom, masterclass | Digital, moderno, pantalla como metáfora |
| **Encuentro presencial** | Carreras grupales, entrenamientos, meetups | Energético, outdoor, comunidad |
| **Taller / Workshop** | Nutrición, mindset, técnica de carrera | Educativo, focalizado, íntimo |
| **Evento de marca** | Lanzamientos, aniversarios, collabs con sponsors | Premium, institucional, celebratorio |

## Datos requeridos (checklist)

**Nunca diseñar sin completar este checklist.** Preguntar al usuario cada dato pendiente:

| Dato | Obligatorio | Notas |
|------|-------------|-------|
| Tipo de evento | Si | Webinar, presencial, taller, o marca |
| Nombre del evento | Si | Título principal de la invitación |
| Fecha | Si | Día de la semana + fecha completa |
| Hora | Si | Incluir zona horaria si el evento es virtual |
| Tema / descripción | Si | 1-2 líneas que expliquen de qué se trata |
| Coach o host | Si | Nombre y rol/título |
| Precio o "Gratis" | Si | Siempre visible. Si es gratis, usar "Entrada libre" o "Gratis" |
| Link de registro | Si | Se usa para generar el código QR |
| Lugar / Plataforma | Si | Dirección si es presencial; plataforma si es virtual |
| Dimensiones | Preguntar | 1080x1080, 1080x1920, o ambas |

## Código QR

**Obligatorio en toda invitación.** El QR se genera automáticamente a partir del link de registro proporcionado por el usuario.

### Reglas del QR
- Generar con la librería `qrcode` de Python (o equivalente disponible) usando el link del usuario
- Color del QR: Verde `#163935` sobre fondo Crema `#F1F1E8`, o Crema sobre Verde
- Tamaño mínimo: 150×150 px en la composición final
- Posición: esquina inferior derecha o zona inferior centrada
- Acompañar con texto "Regístrate aquí" o "Escanea para inscribirte" en Poppins
- Respetar área de silencio del QR (margen blanco alrededor)

## Diseño visual

### Estructura de la invitación (cuadrada 1080×1080)

```
┌──────────────────────────────┐
│  [LOGO 360xRUNNING]         │
│                              │
│  NOMBRE DEL EVENTO           │  ← Poppins Bold, grande
│  Subtítulo / tema            │  ← Poppins Regular
│                              │
│  📅 Fecha                    │
│  🕐 Hora                     │
│  📍 Lugar / Plataforma       │
│  👩 Coach: Nombre            │
│                              │
│  ┌────────┐                  │
│  │  QR    │  GRATIS / $XX    │
│  └────────┘  Regístrate aquí │
└──────────────────────────────┘
```

### Estructura de la invitación (vertical 1080×1920)

```
┌──────────────────────────────┐
│  [LOGO 360xRUNNING]         │
│                              │
│                              │
│  NOMBRE DEL                  │
│  EVENTO                      │  ← Poppins Bold, grande
│                              │
│  Subtítulo / tema            │
│                              │
│  ─────────────────           │
│                              │
│  📅 Fecha                    │
│  🕐 Hora                     │
│  📍 Lugar / Plataforma       │
│  👩 Coach: Nombre            │
│                              │
│  ─────────────────           │
│                              │
│  GRATIS / $XX                │
│                              │
│  ┌────────┐                  │
│  │  QR    │                  │
│  └────────┘                  │
│  Regístrate aquí             │
└──────────────────────────────┘
```

### Reglas de diseño
- **Color de fondo** según categoría del contenido (Entrenamiento = Rosa, Mente = Terracota, Bienestar = Verde, Mixto = Crema)
- **Contraste**: texto siempre legible. Si el fondo es oscuro (Verde/Terracota), texto en Crema. Si el fondo es claro (Rosa/Crema), texto en Verde
- **Logo**: siempre presente, parte superior, respetando área de protección
- **Iconos**: usar iconos simples de línea para fecha, hora, lugar. Mantener dentro de la paleta
- **Fotografía** (opcional): si se usa, debe ser de mujeres en contexto de running/bienestar. Aplicar overlay del color de categoría con opacidad para mantener legibilidad del texto
- **Precio/Gratis**: siempre visible y prominente. Si es gratis, destacar como beneficio

### Tono del copy
- De "tú": "Te esperamos", "Únete", "Reserva tu lugar"
- Directo y energético para eventos presenciales
- Cálido y educativo para talleres
- Premium y aspiracional para eventos de marca
- Nunca genérico: cada invitación debe sentirse como una conversación personal
