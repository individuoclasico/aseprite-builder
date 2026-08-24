# Instrucciones paso a paso - Probar el parche actualizado

Bro, seguí estos pasos exactos. Copiá y pegá cada comando en tu terminal (o Command Prompt en Windows).

## Paso 1: Descargar el código de Aseprite

Abrí una terminal y escribí:

git clone --recurse-submodules -j8 https://github.com/aseprite/aseprite

Esto descarga todo el código en una carpeta llamada "aseprite".

## Paso 2: Entrar a la carpeta

cd aseprite

## Paso 3: Descargar el parche actualizado

En la misma terminal, escribí:

# En Windows (PowerShell):
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/individuoclasico/aseprite-builder/arena/01a03236-aseprite-builder/custom_fps_features.patch" -OutFile "custom_fps_features.patch"

# En Linux / Mac:
 curl -L -o custom_fps_features.patch https://raw.githubusercontent.com/individuoclasico/aseprite-builder/arena/01a03236-aseprite-builder/custom_fps_features.patch

Esto descarga el archivo actualizado.

## Paso 4: Aplicar el parche

git apply --whitespace=fix custom_fps_features.patch

Si no da error, está aplicado correctamente.

## Paso 5: Compilar (como en tu video)

# Si usás Ninja (recomendado):
mkdir build
cmake -S . -B build -G Ninja -DENABLE_TESTS=OFF
cd build
ninja

# Si usás Visual Studio:
cmake -S . -B build
cd build
cmake --build . --config Release

Después de compilar, el archivo ejecutable estará en:
- build/bin/aseprite (Linux/Mac)
- build/bin/Release/aseprite.exe (Windows con VS)
- build/bin/aseprite.exe (Windows con Ninja)

## Paso 6: Probar

Ejecutá el archivo compilado. Deberías ver:
- El checkbox "fps" junto a los 5 botones de play (marcado por defecto).
- Las flechas `<` y `>` junto a la casilla con el número de FPS.
- Al desmarcar el checkbox, los controles FPS se desactivan.

¡Probalo y avisame!
