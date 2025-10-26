# 📝 Instrucciones para Subir a GitHub Pages

## ✅ Ya completado (hecho automáticamente):
- ✓ Repositorio git inicializado
- ✓ Archivo renombrado a `index.html` (requerido para GitHub Pages)
- ✓ Commit inicial creado
- ✓ Rama configurada como `main`
- ✓ Archivos `.gitignore` y `README.md` creados

## 🚀 Pasos para completar la subida:

### Opción 1: Usando GitHub Desktop (Más fácil)

1. **Descarga GitHub Desktop** (si no lo tienes):
   - Ve a: https://desktop.github.com/
   - Descarga e instala

2. **Abre GitHub Desktop**:
   - File → Add Local Repository
   - Selecciona la carpeta: `D:\Proyectos\Diagnostico-Vial_Carlota`
   - Click en "Add Repository"

3. **Publica el repositorio**:
   - Click en "Publish repository" (botón azul arriba)
   - Nombre: `Diagnostico-Vial_Carlota` o el que prefieras
   - Descripción: "Sistema de Reporte de Estado de Vías"
   - ⚠️ Desmarca "Keep this code private" si quieres que sea público
   - Click en "Publish repository"

4. **Activa GitHub Pages**:
   - Ve a tu repositorio en GitHub.com
   - Click en "Settings" (⚙️)
   - En el menú izquierdo, click en "Pages"
   - En "Source", selecciona: `main` branch
   - Click en "Save"
   - ¡Espera 1-2 minutos y tu sitio estará en línea! 🎉

---

### Opción 2: Desde la Terminal (Para usuarios avanzados)

Ejecuta estos comandos en la terminal de PowerShell:

```powershell
# 1. Crear repositorio en GitHub primero en: https://github.com/new
# Nombre sugerido: Diagnostico-Vial_Carlota

# 2. Conectar con tu repositorio de GitHub (reemplaza TU_USUARIO con tu nombre de usuario)
git remote add origin https://github.com/TU_USUARIO/Diagnostico-Vial_Carlota.git

# 3. Subir los archivos
git push -u origin main

# 4. Luego activa GitHub Pages desde la web en Settings → Pages
```

---

### Opción 3: Usando GitHub CLI (gh)

Si tienes GitHub CLI instalado:

```powershell
# 1. Autenticarse (solo primera vez)
gh auth login

# 2. Crear repositorio y subirlo
gh repo create Diagnostico-Vial_Carlota --public --source=. --push

# 3. Activar GitHub Pages
gh repo edit --enable-pages --pages-branch main
```

---

## 🌐 Acceder a tu sitio

Una vez activado GitHub Pages, tu sitio estará disponible en:

```
https://TU_USUARIO.github.io/Diagnostico-Vial_Carlota/
```

Reemplaza `TU_USUARIO` con tu nombre de usuario de GitHub.

---

## ⚠️ Notas Importantes

### Permisos y Funcionalidades:
- **HTTPS requerido**: Algunas funcionalidades requieren HTTPS (GitHub Pages lo proporciona automáticamente)
- **Geolocalización**: Funcionará perfectamente en HTTPS ✓
- **Cámara**: Puede requerir permisos especiales en algunos dispositivos
- **Dictado de voz**: Funciona mejor en Chrome/Edge sobre HTTPS

### Primera vez en GitHub Pages:
- Puede tardar 5-10 minutos en estar disponible
- Si ves un error 404, espera unos minutos y recarga

### Actualizaciones futuras:
Cada vez que quieras actualizar tu sitio:
```powershell
git add .
git commit -m "Descripción de cambios"
git push
```

---

## 🆘 Solución de Problemas

### "Permission denied" al hacer push:
- Usa GitHub Desktop en su lugar, o
- Configura tus credenciales: `gh auth login`

### Sitio muestra código en lugar de la página:
- Verifica que el archivo se llame `index.html`
- Verifica que GitHub Pages esté configurado en la rama `main`

### Los reportes no se guardan:
- Es normal, `localStorage` es local a cada navegador
- Para reportes persistentes, necesitarías un backend

---

## 📱 Compartir tu Proyecto

Una vez publicado, puedes:
- Compartir el enlace con compañeros y profesores
- Generar un código QR para acceso móvil rápido
- Agregar el enlace a tu CV o portafolio

---

**¿Necesitas ayuda?** Consulta la documentación oficial:
- GitHub Pages: https://pages.github.com/
- GitHub Desktop: https://docs.github.com/es/desktop

