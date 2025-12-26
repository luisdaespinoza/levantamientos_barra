# 📊 Levantamiento por Código de Barras (Local)

Una aplicación web ligera, rápida y responsiva diseñada para el escaneo y registro de códigos de barras directamente desde el navegador. Ideal para inventarios rápidos, control de stock o recolección de datos en campo sin necesidad de una infraestructura compleja.

## ✨ Características

* **🔍 Escaneo en Tiempo Real:** Utiliza la librería **ZXing-JS** para detectar múltiples formatos de códigos de barras (EAN-13, Code 128, UPC, etc.) usando la cámara del dispositivo.
* **💾 Persistencia Local:** Los datos se guardan automáticamente en el `localStorage` del navegador, por lo que no perderás la información si recargas la página o cierras el navegador.
* **📱 Diseño Responsivo:** Construido con **Tailwind CSS**, optimizado para su uso en smartphones, tablets y computadoras de escritorio.
* **📋 Gestión de Datos:**
    * Visualización de lista en tiempo real (últimos registros primero).
    * Eliminación individual de registros por fila.
    * Botón para copiar toda la lista al portapapeles (formato de texto plano).
    * Limpieza total de datos con modal de confirmación de seguridad.
* **⚡ Sin Instalación:** Funciona directamente abriendo el archivo HTML. No requiere Node.js, bases de datos ni servidores backend.

## 🚀 Tecnologías Utilizadas

* **HTML5 & JavaScript (ES6+):** Lógica principal y manejo de eventos.
* **[Tailwind CSS](https://tailwindcss.com/):** Estilizado moderno y responsivo vía CDN.
* **[ZXing-JS/Library](https://github.com/zxing-js/library):** Motor de escaneo de alta precisión para diversos formatos.
* **Google Fonts (Inter):** Tipografía optimizada para lectura de datos.

## 🛠️ Instalación y Uso

No requiere instalación de dependencias ni compilación.

1.  Clona este repositorio o descarga el archivo `.html`.
2.  Abre el archivo en tu navegador preferido.
3.  Otorga permisos de acceso a la cámara cuando el navegador lo solicite.
4.  ¡Empieza a escanear!

> [!IMPORTANT]
> **Nota sobre Seguridad:** Para que la cámara funcione en dispositivos móviles, la página debe servirse a través de **HTTPS** (o usar `localhost`), ya que los navegadores modernos bloquean el acceso a dispositivos de captura en sitios no seguros.

## 📋 Formatos Soportados

El sistema está configurado para detectar automáticamente:
* **CODE_128** (Logística y envíos)
* **EAN-13 / EAN-8** (Productos comerciales)
* **UPC-A / UPC-E** (Retail)
* **CODE_39** (Uso industrial)
* **ITF** (Interleaved 2 of 5)
