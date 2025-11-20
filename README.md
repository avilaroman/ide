# IDE GROK

<img width="1570" height="1721" alt="Captura de pantalla 2025-07-10 a la 1:02:20PM" src="https://github.com/user-attachments/assets/58ae9c9e-2aa1-4170-ad3a-1971509fa452" />

*Un entorno de desarrollo elegante con tema oscuro y capacidades avanzadas de IA*

</div>

## 🎯 DESCRIPCIÓN GENERAL

El IDE Grok es un entorno de desarrollo de vanguardia inspirado en las interfaces de Metal Gear Solid. Con una estética elegante en negro y detalles en blanco, este IDE combina las capacidades de codificación tradicionales con la potente asistencia de IA de Grok de xAI.

## ⚡ CARACTERÍSTICAS PRINCIPALES

### 🖥️ **INTERFAZ MODERNA**

- **Tema oscuro inspirado en Metal Gear Solid** con detalles en blanco
- **Paneles redimensionables** para personalizar la distribución del espacio de trabajo

- **Explorador de archivos avanzado** con operaciones de menú contextual

- **Editor de pestañas múltiples** con indicadores de resaltado de sintaxis

- **Monitoreo de estado en tiempo real** con barra de estado del sistema

### 🤖 **INTEGRACIÓN DE GROK AI**

- **Asistente de IA multimodo** (Código, Imagen, Chat)

- **Generación y análisis de código** con capacidad de inserción

- **Generación de imágenes** usando los modelos de imagen de xAI

- **Asistencia contextual** con integración de contenido de archivos

- **Formato de código avanzado** con compatibilidad con Markdown

### 📁 **OPERACIONES CON ARCHIVOS**

- **Acceso nativo al sistema de archivos** mediante la API del sistema de archivos

- **Creación de archivos y carpetas** directamente desde la interfaz
- **Funcionalidad de autoguardado** con seguimiento de modificaciones
- **Guardado por lotes** para varios archivos
- **Actualizaciones en tiempo real del árbol de archivos**

### 🎨 **MEJORA DE CÓDIGO**

- **Inserción de código generado por IA** directamente en el editor
- **Creación de archivos a partir de bloques de código de IA** con las extensiones correctas

- **Operaciones de copia e inserción** para el contenido generado

- **Iconos de archivo con reconocimiento de sintaxis** para una mejor organización

## 🚀 INSTRUCCIONES DE DESPLIEGUE

### Requisitos previos
- Node.js (v14 o superior)

- NPM (Administrador de paquetes de Node)

- Clave API de xAI para la integración con Grok

### Instalación

1. **Clonar el repositorio:**
```bash

git clone <url-del-repositorio>

cd grok-ide
```

2. **Instalar las dependencias:**
```bash

npm install
```

3. **Configurar Entorno:** Crea un archivo `.env` en el directorio raíz:

```env
XAI_API_KEY=tu_clave_api_xai_aquí
PORT=3000

```

### Secuencia de inicio

1. **Inicia el servidor:**

```bash

npm start

```

2. **Accede a la interfaz:**

Abre tu navegador y navega a `http://localhost:3000`

3. **Comienza las operaciones:**

- Haz clic en "ABRIR CARPETA" para cargar tu proyecto

- Usa el asistente de IA para la generación y el análisis de código

- Crea y edita archivos con el editor

## 🎮 CONTROLES

### Operaciones con archivos

- **CTRL/CMD + S**: Guarda el archivo actual

- **CTRL/CMD + SHIFT + S**: Guarda todos los archivos

- **Clic derecho en el explorador**: Menú contextual para crear archivos y carpetas

### Asistente de IA
- **CTRL/CMD + Enter**: Enviar solicitud a la IA

- **Cambio de modo**: Alternar entre los modos Código, Imagen y Chat

- **Inclusión de contexto**: Incluir el contenido del archivo actual en las solicitudes a la IA

### Editor

- **Gestión de pestañas**: Hacer clic en las pestañas para cambiar de archivo, × para cerrar

- **Guardado automático**: Guardado automático con indicadores de modificación

- **Inserción de código**: Inserción directa desde bloques de código generados por la IA

## 🛠️ ARQUITECTURA

``` Documentación
```

## 🔧 PUNTOS DE ENLACE DE LA API

### Operaciones de IA

- `POST /api/completion` - Autocompletado de chat Grok
- `POST /api/generate-image` - Generación de imágenes con IA

- `POST /api/analyze-code` - Análisis y revisión de código

- `POST /api/analyze-project` - Análisis de la estructura del proyecto

### Operaciones del sistema

- `GET /api/health` - Comprobación del estado del sistema

- `GET /` - Interfaz principal

- `GET /legacy` - Acceso a la interfaz heredada

## 🎨 TEMA

La interfaz utiliza una paleta de colores cuidadosamente diseñada:

- **Negro primario**: `#0a0a0a` - Fondo principal

- **Negro secundario**: `#111111` - Fondos de paneles

- **Negro terciario**: `#1a1a1a` - Fondos de componentes

- **Blanco** Características destacadas**: `#ffffff` - Acentos y bordes
- **Texto turquesa**: `#40e0d0` - Texto de estado discreto

## 🔒 PROTOCOLOS DE SEGURIDAD

- Protección de claves API mediante variables de entorno
- Validación y saneamiento de solicitudes
- Manejo de errores con información del sistema
- Operaciones seguras del sistema de archivos

## 🚨 SOLUCIÓN DE PROBLEMAS

### Problemas comunes

**Funciones de IA que no funcionan:**

- Verifique que XAI_API_KEY esté configurado en el archivo .env
- Compruebe la validez y los permisos de la clave API

- Asegúrese de tener conexión a internet para las solicitudes de IA

**Acceso al sistema de archivos denegado:**

- Use un navegador moderno compatible con la API del sistema de archivos

- Otorgue los permisos necesarios cuando se le solicite

- Asegúrese de usar HTTPS en entornos de producción

**Problemas de rendimiento:**

- Cierre las pestañas que no utilice para liberar memoria

- Limite el tamaño del contexto de IA para archivos grandes

- Use las herramientas para desarrolladores del navegador para supervisar el rendimiento

## 🎯 OBJETIVOS

- [x] Implementación del tema oscuro
- [x] Integración de asistente de IA multimodo
- [x] Operaciones avanzadas con archivos
- [x] Generación e inserción de código
- [x] Capacidades de generación de imágenes
- [x] Interfaz redimensionable
