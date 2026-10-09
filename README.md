# Infobase El Mensaje LVC — La Voz de Consumación

**Infobase LVC** es la biblioteca digital gratuita de **El Mensaje** (*The Message*) del hermano **William Marrion Branham**, creada por **LVC (La Voz de Consumación)**. Reúne en una sola aplicación los sermones del Hermano Branham, la Biblia en varios idiomas y herramientas de estudio bíblico: interlineal hebreo y griego con números Strong, diccionarios, atlas bíblico, medidas y pesos, notas, marcadores y búsqueda global.

Disponible para **Windows, Android, Linux y macOS**, en español, inglés, portugués, francés, italiano, rumano, chino y árabe.

> **The Message — William Marrion Branham sermons, Bible and study tools in one free app.** Infobase LVC lets you read and search the sermons of Brother Branham (89 languages via messagehub.info), the Bible with Strong's interlinear, dictionaries and a Bible atlas. Download the installer for Windows, Android, Linux or macOS from the [Releases](../../releases/latest) page.

> Este repositorio **solo aloja los instaladores** de cada versión publicada.

**Palabras clave:** infobase, LVC, La Voz de Consumación, El Mensaje, The Message, William Marrion Branham, William Branham, sermones, mensajes, Biblia, Bible, interlineal, Strong, atlas bíblico, messagehub.

---

## Descargar la última versión

Ve a **[Releases → última versión](../../releases/latest)** y descarga el archivo de tu sistema:

| Sistema | Archivo |
|---|---|
| Windows | `infobaselvc_vX.Y.Z.exe` |
| Android | `infobaselvc_vX.Y.Z.apk` |
| Linux | `infobaselvc_vX.Y.Z_linux-x64.tar.gz` (+ firma `.asc`) |
| macOS | `.zip` (sin firmar) |

**Windows:** ejecuta el instalador, elige el idioma (Español / English) y sigue el asistente. Se instala en `%LOCALAPPDATA%\Programs\LVC\Infobase\`.

**Actualizaciones automáticas:** la app comprueba cada 6 horas si hay una versión nueva en este repositorio. Cuando aparece, verás un banner con el botón "Actualizar"; tus datos personales se conservan.

---

## Primer arranque

Al abrir la app por primera vez, la pantalla de carga importa los datos base a la base de datos local (`%APPDATA%\LVC\Infobase\db\biblioteca.db`):

- Idiomas (ISO 639-2)
- Interlineal griego y hebreo (Strong)
- Referencias cruzadas bíblicas
- Imágenes y referencias del atlas
- Medidas y pesos bíblicos

---

## Interfaz: las 4 secciones principales

La barra lateral izquierda tiene 4 botones:

| Icono | Sección |
|---|---|
| 📖 | **Biblioteca** — árbol de carpetas/libros (mensajes y biblias) |
| ⬇ | **Descargas** — añadir biblias, mensajes y atlas |
| 🧬 | **Interlineal** — Biblia palabra a palabra con Strong |
| 🗺 | **Atlas** — mapas bíblicos navegables |

---

## Sección Biblioteca

### Árbol de contenido
El panel izquierdo muestra carpetas y libros en árbol. Las carpetas raíz traducidas automáticamente al idioma de la UI (Mensajes/Messages/Mensagens…).

- **Click** en un libro: lo abre en una pestaña.

### Pestañas de lectura
Cada libro abierto vive en una pestaña arriba del editor. Cierra con la X o Click-Derecho "Cerrar Pestaña".

### Buscador global
Barra superior. Busca en el texto plano de todos los libros. Toggles:
- **Aa**: distinguir mayúsculas/minúsculas
- **W**: palabra exacta

Los resultados se resaltan en amarillo dentro de cada libro al abrirlo.

### Editor de libros (vista lectura)

Cuando abres un libro, dispones de la barra superior con:

- **Tamaño de letra `−` / `+`**: aumenta o disminuye el tamaño del texto. Rango 70 % – 200 % en pasos de 10 %. El tamaño elegido se persiste y se aplica a todos los libros.
- **🔍 Buscar en el libro**: buscador local con resaltado.
- **📝 Notas**: panel lateral con tus notas por párrafo.
- **🔖 Marcadores**: panel lateral con tus marcadores.

#### Selección de párrafos
Para mensajes/sermones, al hacer click en el margen izquierdo de un párrafo numerado se selecciona ese párrafo. Aparece una barra flotante para copiar el texto seleccionado con referencias.

#### Funciones específicas de capítulos bíblicos
Cuando abres un capítulo de la Biblia:
- **📖 Biblia paralela** — compara con otra traducción lado a lado
- **↔ Comparar versiones** — diferencias entre traducciones del mismo capítulo
- **🌐 Interlineal** — abre la palabra-por-palabra de ese capítulo
- **🔗 Referencias cruzadas** — versículos relacionados en otras partes
- **🗺 Atlas** — mapas relacionados con ubicaciones del capítulo

---

## Sección Descargas

Tres pestañas: **Biblias**, **Atlas**, **Mensajes**. Verifica conexión a internet al entrar; si no hay, muestra aviso y desactiva las descargas.

### Pestaña Biblias

- Lista de idiomas con biblias disponibles en el repo público de catálogo.
- Click en un idioma → despliega la lista de traducciones de ese idioma.
- Cada traducción muestra tamaño y un botón de descarga.
- Las traducciones ya instaladas tienen marca verde.
- Al descargar, se importa al árbol de carpetas como `Biblias / Idioma / Versión / Libro / Capítulo`.

### Pestaña Atlas

- Si nunca lo descargaste, botón **"Instalar atlas"**.
- Descarga ~700 mapas e imágenes.
- El progreso se muestra con barra y contador.
- Una vez instalado, "Reinstalar" baja la versión más reciente.

### Pestaña Mensajes

Dos sub-pestañas:

#### ⚡ Curados (formato completo)
- Mensajes traducidos manualmente por LVC, con formato preservado (negrita, cursiva, sub-párrafos).
- Catálogo limitado a los idiomas que LVC ha procesado.
- Estructura de carpetas: `Mensajes / ES / 1965 / "65-0418M Eventos modernos aclarados por la profecía"`.

#### ☁ Catálogo Messagehub
- **89 idiomas** disponibles desde messagehub.info.
- Texto plano (sin negrita/cursiva).
- Estructura: `Mensajes / Messagehub / IDIOMA / AÑO / "47-1102 El Ángel Y Su Comisión"`.

**El botón `↻` recarga el catálogo** invalidando la caché local (TTL 3 días) — útil cuando hay nuevos mensajes en el repo.

---

## Sección Interlineal

Lectura de la Biblia palabra-por-palabra con análisis morfológico:

- Selector de **libro** (Génesis → Apocalipsis) y **capítulo**.
- Cada versículo muestra:
  - La palabra original (hebreo o griego) con dirección RTL para hebreo.
  - Código **Strong** (G/H + número) clickable: abre el diccionario.
  - Morfología (parsing gramatical).
  - Traducción literal.
- Selector de **idioma de la morfología/traducción** (multilenguaje).

---

## Sección Atlas

Mapas bíblicos navegables.

- Pestañas: **Antiguo Testamento**, **Nuevo Testamento**, **Otros Atlas**, **Líneas del Tiempo**.
- Carpetas → desplegables → imágenes ordenadas naturalmente.
- Click en una miniatura → vista grande con zoom y arrastre.
- Las imágenes referenciadas desde un capítulo bíblico se muestran con la herramienta **🗺** del editor.

---

## Notas y marcadores (por libro)

### Notas
- En vista de lectura, click en el icono **📝**.
- Sidebar lateral con notas existentes por párrafo.
- Click en un párrafo + escribir nota → se asocia automáticamente.
- Las notas se exportan/importan junto con el libro.

### Marcadores
- Icono **🔖** en la barra superior del libro.
- Click en margen izquierdo de un párrafo → toggle marcador.
- Lista global de marcadores accesible desde el menú principal.

---

## Configuración (esquina superior derecha)

- **🌓 Tema** — claro / oscuro.
- **🌐 Idioma de la app** — Español, English, Português, Français, Română, Italiano.

El idioma de la UI se guarda y se aplica al reiniciar.

---

## Atajos de teclado

| Atajo | Acción |
|---|---|
| Ctrl + F | Buscar dentro del libro abierto |
| Esc | Cerrar buscador local / cancelar edición |
| Ctrl + Shift + F | Buscador global (en barra superior) |

---

## Solución de problemas

- **No detecta actualizaciones** → revisa conexión a internet. Espera al check siguiente (cooldown 6h) o reinicia la app.
- **Búsqueda no encuentra nada en biblias descargadas** → el índice FTS se reconstruye en background. Espera unos segundos tras importar.
- **Mensaje "carpeta vacía" en Atlas** → entra a Descargas → Atlas → Instalar. Las imágenes se descargan de internet.

---

## Sobre las versiones

Numeración semver `X.Y.Z`:
- **X** mayor: cambios estructurales (migración DB grande, rediseño UI).
- **Y** menor: features nuevas (nuevos idiomas, nuevos paneles).
- **Z** parche: bugfixes.

La app comprueba este repositorio cada 6 horas. Puedes descartar una versión con "Después"; no volverá a aparecer hasta la siguiente.

---

*Copyright © LVC. Esta app no es producto oficial de Voice of God Recordings ni de messagehub.info. Los textos del Hermano Branham se utilizan bajo el espíritu de difusión libre del Mensaje.*
