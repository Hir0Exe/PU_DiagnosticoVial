# 🛣️ ReportVías - Sistema de Reporte de Estado de Vías

Sistema web demostrativo para reportar problemas en vías públicas utilizando tecnologías modernas de HTML5.

## ✨ Funcionalidades Implementadas

### 📍 Geolocalización en Tiempo Real
- Botón de ubicación actual que usa la **Geolocation API** de HTML5
- Centra automáticamente el mapa en tu ubicación
- Marcador visual para tu posición actual
- Solicita permisos de ubicación al usuario

### 🔍 Búsqueda de Lugares
- Buscador integrado en el mapa
- Usa **Nominatim** (servicio de OpenStreetMap) para geocodificación
- Busca direcciones, lugares y puntos de interés
- Resultados optimizados para Cúcuta, Colombia

### 🏷️ Selección de Tipo de Problema
- Botones visuales predeterminados con iconos
- 6 categorías principales:
  - 🛣️ Baches
  - ⚡ Grietas en el pavimento
  - 🚦 Problemas de señalización
  - 💡 Falta de iluminación
  - 💧 Problemas de drenaje
  - ➕ Otros
- Interfaz intuitiva con feedback visual

### 📷 Captura de Foto
- Acceso directo a la cámara del dispositivo
- Opción de seleccionar desde galería
- Vista previa de la imagen antes de enviar
- Validación de tamaño (máx. 5MB)
- Almacenamiento en Base64 para persistencia local

### 🎤 Dictado de Voz
- Reconocimiento de voz usando **Web Speech API**
- Idioma configurado en español (es-ES)
- Botón intuitivo con animación durante grabación
- Transcripción en tiempo real
- Compatible con Chrome, Edge y Safari

### 📱 Diseño Responsive
- Optimizado para dispositivos móviles
- Adaptación automática a diferentes tamaños de pantalla
- Controles táctiles optimizados
- Meta tags para mejor experiencia en iOS y Android
- Prevención de zoom no deseado en inputs

### 💾 Almacenamiento Local
- Todos los reportes se guardan en `localStorage`
- Las fotos se almacenan como Base64
- Persistencia entre sesiones
- Exportación de datos en formato JSON

### ✅ Sistema de Validación Comunitaria
- Votación de reportes (Verídico/No Verídico)
- Estadísticas en tiempo real
- Prevención de múltiples votos por usuario
- Contador de validaciones

## 🚀 Cómo Usar

### Instalación
1. Descarga el archivo `reporte_vias.html`
2. Abre el archivo en un navegador web moderno

### Uso Básico

#### 1️⃣ Encontrar la Ubicación
- **Opción A**: Haz clic en el botón 🎯 para usar tu ubicación actual
- **Opción B**: Escribe una dirección en el buscador del mapa

#### 2️⃣ Crear un Reporte
- Haz clic en el mapa donde hay un problema
- Selecciona el tipo de problema con los botones visuales
- Describe el problema (escribe o usa dictado de voz)
- Opcionalmente toma una foto
- Envía el reporte

#### 3️⃣ Validar Reportes
- Revisa los reportes de otros usuarios
- Marca como "Verídico" o "No Verídico"
- Ayuda a la comunidad a identificar problemas reales

### Funciones Administrativas
- **Exportar JSON**: Descarga todos los reportes en formato JSON
- **Limpiar Todo**: Elimina todos los reportes almacenados

## 📋 Requisitos del Sistema

### Navegadores Compatibles
- ✅ **Google Chrome** (recomendado) - Todas las funcionalidades
- ✅ **Microsoft Edge** - Todas las funcionalidades
- ⚠️ **Safari** - Funcionalidades completas (iOS/macOS)
- ⚠️ **Firefox** - Algunas limitaciones en reconocimiento de voz

### Permisos Necesarios
- 📍 **Ubicación**: Para geolocalización
- 📷 **Cámara**: Para captura de fotos
- 🎤 **Micrófono**: Para dictado de voz

### Dispositivos Compatibles
- 📱 Smartphones (Android/iOS)
- 💻 Tablets
- 🖥️ Computadores de escritorio

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Diseño responsive con gradientes y animaciones
- **JavaScript ES6+**: Lógica de la aplicación
- **Leaflet.js**: Mapas interactivos
- **OpenStreetMap**: Tiles del mapa y geocodificación (Nominatim)
- **Bootstrap 5**: Componentes UI (modal, alertas)
- **Font Awesome 6**: Iconografía

### APIs HTML5
- **Geolocation API**: Ubicación en tiempo real
- **Web Speech API**: Reconocimiento de voz
- **File API**: Lectura de imágenes
- **LocalStorage API**: Persistencia de datos

## 📊 Estructura de Datos

### Formato de Reporte
```json
{
  "id": 1234567890,
  "lat": 7.8939,
  "lng": -72.5078,
  "description": "Bache profundo en la vía",
  "type": "baches",
  "photo": "data:image/jpeg;base64,...",
  "timestamp": "2024-10-26T10:30:00.000Z",
  "validations": {
    "veridico": 5,
    "noVeridico": 1
  },
  "userValidated": false
}
```

## 🎨 Características de Diseño

- Gradiente moderno (púrpura a violeta)
- Tarjetas con sombras y efectos hover
- Iconos intuitivos de Font Awesome
- Animaciones CSS suaves
- Tema de colores coherente
- Feedback visual para todas las acciones

## 🔒 Privacidad y Seguridad

- Todos los datos se almacenan localmente en el navegador
- No hay envío de datos a servidores externos (excepto geocodificación)
- Las fotos permanecen en el dispositivo del usuario
- Cumple con mejores prácticas de privacidad

## 📝 Notas Importantes

### Reconocimiento de Voz
- Funciona mejor en lugares con poco ruido
- Requiere conexión a internet (procesamiento en la nube)
- En Chrome, puede requerir HTTPS en producción

### Almacenamiento
- El `localStorage` tiene un límite (~5-10MB)
- Las fotos grandes pueden alcanzar este límite
- Se recomienda exportar y limpiar datos periódicamente

### Geolocalización
- La precisión depende del dispositivo y la señal GPS
- En interiores puede ser menos precisa
- Requiere permisos del usuario

## 🎓 Uso Académico

Este proyecto es ideal para:
- Demostraciones de tecnologías web modernas
- Proyectos universitarios de ingeniería de sistemas
- Aprendizaje de APIs de HTML5
- Estudios de UX/UI en aplicaciones móviles
- Proyectos de impacto social

## 📞 Información del Proyecto

- **Tipo**: Proyecto Universitario - Página Demostrativa
- **Ubicación**: Cúcuta, Norte de Santander, Colombia
- **Propósito**: Demostración de funcionalidades web modernas
- **Enfoque**: Aplicación web progresiva (PWA-like)

## 🆘 Solución de Problemas

### La geolocalización no funciona
- Verifica que hayas dado permisos de ubicación al navegador
- En algunos navegadores, requiere HTTPS (no HTTP)
- Comprueba la configuración de privacidad del dispositivo

### El dictado de voz no responde
- Asegúrate de usar Chrome, Edge o Safari
- Verifica permisos de micrófono
- Requiere conexión a internet
- Prueba en un ambiente con menos ruido

### La cámara no se activa
- Da permisos de cámara al navegador
- En iOS, asegúrate de usar Safari o Chrome
- Verifica que ninguna otra app esté usando la cámara

### Las fotos no se guardan
- El archivo puede ser muy grande (límite 5MB)
- El `localStorage` puede estar lleno
- Intenta limpiar reportes antiguos

## 🔄 Futuras Mejoras Posibles

- Backend para almacenamiento centralizado
- Autenticación de usuarios
- Notificaciones push
- Modo offline completo (PWA)
- Integración con APIs gubernamentales
- Sistema de chat entre usuarios
- Filtros por tipo de problema
- Mapa de calor de problemas
- Reportes con múltiples fotos

## 📄 Licencia

Proyecto educativo de código abierto. Libre para uso académico y demostrativo.

---

**Desarrollado con ❤️ para la comunidad de Cúcuta**

Para soporte o preguntas sobre el proyecto, consulta la documentación en el código fuente.

