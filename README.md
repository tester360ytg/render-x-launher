#🚀 RenderX Launcher

RenderX Launcher es un lanzador avanzado de juegos para Windows que permite ejecutar títulos usando backends gráficos por software y simular GPUs. Ideal para PCs con tarjetas gráficas limitadas o ausentes, combinando compatibilidad, personalización y facilidad de uso.

Con RenderX puedes:

Elegir motores de render por software: Direct3D WARP, Mesa llvmpipe/OpenGL, Lavapipe/SwiftShader Vulkan.

Simular GPU con nombre, VRAM y vendor.

Guardar configuraciones persistentes para cada juego en Documentos del usuario.

Lanzar juegos automáticamente con todas las opciones aplicadas.

#🎨 Características principales
1️⃣ Backends gráficos

✅ Direct3D WARP

✅ Mesa llvmpipe (OpenGL)

✅ Lavapipe Vulkan

✅ SwiftShader Vulkan

Copiado automático de DLL/JSON al directorio del juego.

Selección de driver personalizada por backend.

#2️⃣ GPU Spoofing

Simula:

Nombre de GPU

VRAM

Vendor (Intel, AMD, NVIDIA)

Configuración persistente por juego.

#3️⃣ Configuraciones persistentes

Guardadas en:
Documentos/RenderXLauncher/config.json

Mantiene backend, DLL y GPU spoofing por juego.

Listado de juegos configurados para fácil selección.

#4️⃣ Interfaz gráfica amigable (Tkinter)

Comboboxes para backend, GPU, VRAM y vendor.

Botones intuitivos: seleccionar EXE, driver, guardar GPU y lanzar juego.

Mensajes claros de error y éxito.

#📝 Guía de uso
#1️⃣ Seleccionar un juego

Haz clic en 📂 Seleccionar EXE.

Elige el ejecutable del juego (.exe).

El launcher actualizará el listado de juegos disponibles.

#2️⃣ Elegir backend

Selecciona el backend deseado.

Haz clic en ⚙️ para elegir el DLL/JSON correspondiente.

#3️⃣ Configurar GPU Spoofing

Selecciona el nombre de GPU, VRAM y vendor.

Haz clic en 💾 Guardar GPU Spoof para mantener la configuración.

#4️⃣ Lanzar juego

Haz clic en 🚀 Lanzar Juego.

RenderX ajustará automáticamente el entorno y ejecutará el juego.

#⚠️ Aclaraciones y límites

Compatibilidad: Solo Windows.

Backends por software: Dependen del CPU; no hay aceleración por GPU real.

GPU spoofing: Solo afecta variables de entorno visibles para el juego.

DLL/JSON: Deben existir en las carpetas correspondientes (dll/).

VRAM máximo: Hasta 24 GB, limitado por el soporte del juego y CPU.

Seguridad: No modifica archivos del sistema ni instala drivers.

#📂 Estructura de carpetas
RenderXLauncher/
├─ dll/
│  ├─ dxwarp/
│  ├─ opengl/
│  ├─ lavapipe/
│  └─ vk/
├─ renderx_launcher.py
└─ Documents/RenderXLauncher/config.json

#🔧 Requisitos para copilar

Python 3.8 o superior

Tkinter (incluido en Python estándar)

Juegos compatibles con backends por software

#💡 Tips & Trucos

Siempre selecciona un DLL válido antes de lanzar un juego.

Guarda la configuración de GPU antes de cerrar el launcher.

Experimenta con distintos backends para optimizar rendimiento en tu CPU.

RenderX funciona mejor en juegos que soportan modo software rendering.
