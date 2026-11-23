<div align="center">

  <!-- MARCADOR DE POSICIÓN PARA BANNER / LOGO DEL PROYECTO -->
  <img src="assets/banner.png" alt="LiquidGlass LSPosed Banner" width="100%" />

  # LiquidGlass para WhatsApp e Instagram (Módulo LSPosed)

  **Transforma la interfaz de WhatsApp e Instagram en dispositivos Samsung en una estética elegante y moderna de LiquidGlass de forma dinámica, sin modificar los APK originales.**

  [![Android](https://img.shields.io/badge/Android-16%2B-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com/)
  [![Device](https://img.shields.io/badge/Samsung-Rooted-1428A0?style=for-the-badge&logo=samsung&logoColor=white)](https://www.samsung.com/)
  [![LSPosed API](https://img.shields.io/badge/LSPosed%20API-101%20--%20103-blue?style=for-the-badge)](https://github.com/LSPosed/LSPosed)
  [![WhatsApp](https://img.shields.io/badge/WhatsApp-Soporte%20Beta-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://www.whatsapp.com/)
  [![Instagram](https://img.shields.io/badge/Instagram-Próximamente-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/)
  [![License](https://img.shields.io/badge/License-GPLv3-orange?style=for-the-badge)](LICENSE)

  <p align="center">
    <a href="README.md">🇺🇸 English</a> •
    <a href="README_ID.md">🇮🇩 Bahasa Indonesia</a> •
    <a href="README_ES.md">🇪🇸 Español</a>
  </p>

</div>

---

## 📖 Descripción General

**LiquidGlass** es un módulo avanzado de Xposed/LSPosed diseñado específicamente para dispositivos Samsung rooteados con versiones modernas de Android. Al inyectarse (*hooking*) directamente en el proceso de renderizado de la interfaz de usuario (UI) de la aplicación en tiempo de ejecución, este módulo aplica efectos de **desenfoque translúcido en tiempo real, glassmorphism y refracción líquida** (LiquidGlass) a **WhatsApp** (actualmente en Beta) e **Instagram** (próximamente).

Dado que funciona exclusivamente mediante *Xposed hooking*, **no requiere parchar, reempaquetar ni clonar los APK**. Tus aplicaciones permanecen 100% originales, seguras y compatibles con las actualizaciones oficiales de Google Play Store.

---

## 🎬 Vista Previa (Preview)

> *Reemplaza las rutas de marcador de posición a continuación con tus archivos `.gif` o `.mp4` reales dentro de la carpeta `assets/` de tu repositorio.*

<div align="center">
  <table>
    <tr>
      <td align="center"><b>WhatsApp (Beta)</b></td>
      <td align="center"><b>Instagram (Próximamente)</b></td>
    </tr>
    <tr>
      <td><img src="assets/preview_whatsapp.gif" alt="Vista previa de WhatsApp LiquidGlass" width="320"/></td>
      <td><img src="assets/preview_instagram.gif" alt="Vista previa de Instagram LiquidGlass" width="320"/></td>
    </tr>
  </table>
</div>

---

## ✨ Características Principales y Hoja de Ruta

- **Cero Modificación de APK:** Realiza *hooks* directamente en las vistas de la UI en tiempo de ejecución, conservando las firmas digitales originales de las aplicaciones.
- **Desenfoque Dinámico en Tiempo Real:** Fondos translúcidos acelerados por hardware con radio de desenfoque, opacidad de tinte y radio de esquinas personalizables.
- **Integración con WhatsApp (🧪 Beta):** Aplica fondos de chat translúcidos, barras superiores/de navegación esmeriladas y ventanas modales de cristal en las últimas versiones globales de WhatsApp.
- **Integración con Instagram (⏳ Próximamente):** El soporte para el feed de Instagram, mensajes directos (DM) y barras de navegación translúcidas se encuentra actualmente en desarrollo activo.
- **Ligero y Eficiente en Batería:** Utiliza las API nativas `RenderEffect` de Android y las API de desenfoque propias de Samsung para garantizar fluidez y bajo consumo.

---

## 📱 Dispositivos Compatibles y Requisitos

Para garantizar un rendimiento y estabilidad óptimos, verifica que tu dispositivo cumpla con los siguientes requisitos:

| Componente | Requisito / Compatibilidad |
| :--- | :--- |
| **Marca del Dispositivo** | Dispositivos Samsung Galaxy Rooteados (Series S, Z, Note y Serie A) |
| **Versión del SO** | **Android 16+** (OneUI 8.0 / 8.1 o superior) |
| **Solución Root** | Magisk (v27+), KernelSU o APatch |
| **Framework** | **LSPosed** (Zygisk / NeoZygisk) compatible con **API 101 – 103** |
| **Apps Compatibles** | **WhatsApp (Global - Beta)** e **Instagram (Próximamente)** |

> **⚠️ Nota:** Los dispositivos que no sean Samsung o las Custom ROM basadas en AOSP **no son compatibles oficialmente**, ya que este módulo utiliza las API nativas de desenfoque de Samsung.

---

## 🚀 Instalación y Uso

1. **Requisitos Previos:** Asegúrate de que tu dispositivo Samsung esté rooteado y tenga instalado y activo **LSPosed (API 101–103)**.
2. **Descarga:** Descarga la última versión de `LiquidGlass-vX.X.apk` desde la sección [Releases](../../releases).
3. **Instalación:** Instala el archivo APK descargado como una aplicación normal.
4. **Activar el Módulo:**
   - Abre **LSPosed Manager**.
   - Ve a la pestaña **Módulos** y activa **LiquidGlass**.
   - En la lista de ámbito (*Scope*), selecciona **WhatsApp** *(e **Instagram** cuando esté disponible)*.
5. **Aplicar Cambios:**
   - **Fuerza la detención** de WhatsApp desde los ajustes del dispositivo y vuelve a abrirlo para ver el efecto LiquidGlass.
6. **Personalización (Opcional):** Abre la aplicación complementaria **LiquidGlass** desde tu cajón de aplicaciones para ajustar la intensidad del desenfoque, el tinte del cristal y los bordes.

---

## 🛠️ Solución de Problemas (Troubleshooting)

<details>
<summary><b>1. El efecto LiquidGlass no aparece en WhatsApp.</b></summary>
<br>
- Verifica que **WhatsApp** esté marcado dentro del **Ámbito (Scope) del Módulo en LSPosed**.
- Asegúrate de haber **Forzado la detención** de WhatsApp después de activar el módulo.
- Comprueba que tu framework LSPosed esté ejecutando la **API 101 a 103**. Las versiones antiguas de LSPosed no pueden inyectarse en las vistas de Android 16+.
</details>

<details>
<summary><b>2. WhatsApp se cierra inesperadamente (Crash) tras actualizar desde Play Store (Aviso Beta).</b></summary>
<br>
- Dado que el soporte para WhatsApp está en fase **Beta** y WhatsApp suele ofuscar sus clases internas con frecuencia, una nueva actualización global puede romper los *hooks*. Si ocurre un cierre forzoso, desmarca WhatsApp temporalmente en el Scope de LSPosed y revisa la pestaña [Releases](../../releases) o [Issues](../../issues) para descargar una actualización.
</details>

<details>
<summary><b>3. Lentitud o caída de fotogramas (lag) al desplazarse por los chats.</b></summary>
<br>
- Abre la **Aplicación Complementaria LiquidGlass** y reduce el **Radio de Desenfoque** o desactiva la **Refracción en Tiempo Real** en dispositivos Galaxy Serie A de gama media.
- Asegúrate de que la opción *Desactivar superposiciones HW* esté **desactivada** en las Opciones de Desarrollador de Android.
</details>

<details>
<summary><b>4. Error "LSPosed API Mismatch" o el módulo no logra inicializarse.</b></summary>
<br>
- Este módulo está compilado estrictamente para **LSPosed API 101–103** en Android 16+. Actualiza tus versiones de Zygisk y LSPosed a las últimas compilaciones compatibles.
</details>

---

## 🤝 Contribuciones y Reporte de Errores

¡Las contribuciones, solicitudes de funciones y reportes de errores son bienvenidos!
- ¿Encontraste un error en la Beta de WhatsApp? Abre un [Issue](../../issues) y adjunta tus **Registros (Logs) de LSPosed** junto con el **Modelo exacto de tu dispositivo, Versión de OneUI y Versión de WhatsApp**.

---

## 📜 Aviso Legal y Licencia

- **Aviso Legal:** Este módulo se proporciona *"tal cual"*. Rootear tu dispositivo Samsung anula la garantía de Samsung Knox. El desarrollador no se hace responsable de *bootloops*, inestabilidad del sistema o problemas con aplicaciones de terceros.
- **Licencia:** Distribuido bajo la licencia **GNU General Public License v3.0 (GPLv3)**. Consulta el archivo `LICENSE` para más detalles.