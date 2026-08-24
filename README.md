# Aseprite_Fps Builder 🎨⏱️

Compilador automático de **Aseprite_Fps** personalizado mediante **GitHub Actions**.

---

## ✨ Novedades y Modificaciones Incluidas

### 1. ⏱️ Casilla y Controles de FPS (Línea de Tiempo)
* **`[ < ]` (Flecha izquierda):** Disminuye **-1 FPS** (Límite mínimo: **4 FPS**).
* **`[ 12 fps ]` (Casilla interactiva):** Muestra los FPS calculados según la duración del frame. Puedes hacer clic y escribir directamente cualquier valor numérico deseado, o usar la rueda del ratón. Convierte automáticamente a milisegundos y actualiza el sprite.
* **`[ > ]` (Flecha derecha):** Aumenta **+1 FPS**.

### 2. 🎞️ Creación Rápida de Fotogramas (4 botones)
* **`[ <-F ]` :** Duplica el fotograma actual y lo inserta **a la izquierda** (antes del actual).
* **`[ F-> ]` :** Duplica el fotograma actual y lo inserta **a la derecha** (después del actual, equivalente a `Alt+N`).
* **`[ <-B ]` :** Inserta un nuevo fotograma en blanco **a la izquierda** (antes del actual).
* **`[ B-> ]` :** Inserta un nuevo fotograma en blanco **a la derecha** (después del actual, equivalente a `Alt+B`).

### 3. 📑 Gestión de Capas
* **`[ +Lay ]` :** Crea una nueva capa inmediatamente **abajo** de la capa activa seleccionada.

### 4. 🔄 Herramientas de Transformación
* **`[ FlipH ]` :** Voltea horizontalmente la selección activa o el lienzo completo (`Shift+H`).
* **`[ FlipV ]` :** Voltea verticalmente la selección activa o el lienzo completo (`Shift+V`).
* **`[ Rot- ]` :** Rota el sprite **-90°** (sentido antihorario).
* **`[ Rot+ ]` :** Rota el sprite **+90°** (sentido horario).

### 5. 👁️ Previsualización Rápida
* **`[ Prev ]` :** Abre o cierra la ventana flotante de previsualización (`F7`).
* **`[ Full ]` :** Abre la previsualización a pantalla completa (`F8`).

### 6. 🇪🇸 Paquete de Idioma en Español Integrado
* Incluye la extensión oficial en español (`Español`).
* Para activarlo: En Aseprite ve a `Edit > Preferences > General > Language` (o `Edición > Preferencias`) y selecciona **Español**.

### 7. 🏷️ Identificación
* El programa y su ventana se identifican como **`Aseprite_Fps`**.

---

## 🚀 ¿Cómo compilar y descargar tu versión en GitHub?

1. En la parte superior de tu repositorio, haz clic en la pestaña **Actions**.
2. En la lista de la izquierda, haz clic en **`Build and release Aseprite`**.
3. Haz clic en el botón desplegable **`Run workflow`** a la derecha y luego presiona el botón verde **`Run workflow`**.
4. GitHub comenzará a compilar automáticamente en Windows, Mac y Linux (toma unos 8 a 12 minutos).
5. Cuando termine, ve a la sección **Releases** (a la derecha de la página principal del repositorio) y descarga el archivo `.zip` para tu sistema operativo (ejemplo: `Aseprite_Fps-v1.3.x-Windows.zip`).
6. ¡Descomprime el `.zip` y abre `aseprite.exe`!
