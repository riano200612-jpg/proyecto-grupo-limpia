# 🚀 Subir Proyecto a GitHub

## ✅ Tu Proyecto Está Listo

El proyecto local ya contiene **3 commits** y está preparado para GitHub:

```
5a0a408 - Mejorar: Bajar botones del header, optimizar carga de videos
83a47a6 - Agregar guía de configuración de GitHub
38711a9 - Initial commit: Proyecto Grupo Limpia
```

---

## 📋 Pasos para Subir a GitHub

### 1️⃣ Crear Repositorio en GitHub

1. Abre https://github.com/new
2. Rellena:
   - **Repository name:** `proyecto-grupo-limpia`
   - **Description:** Sitio web de limpieza corporativa premium en Cartagena
   - **Público** (activado)
3. **NO marques** "Initialize this repository"
4. Haz clic en **"Create repository"**

### 2️⃣ Ejecuta en tu Terminal

Reemplaza `TU_USUARIO` con tu usuario de GitHub:

```bash
cd /home/riano200612/proyecto-grupo-limpia

# Renombrar rama a main
git branch -M main

# Conectar con GitHub
git remote add origin https://github.com/TU_USUARIO/proyecto-grupo-limpia.git

# Hacer push
git push -u origin main
```

### 3️⃣ Autenticación

Cuando Git te pida contraseña/token:

**Opción A - Personal Access Token (Recomendado):**
- Ve a: https://github.com/settings/tokens/new
- Crea un token con permiso `repo`
- Usa el token como contraseña

**Opción B - SSH:**
```bash
ssh-keygen -t ed25519 -C "tu-email@example.com"
# Luego agrega la clave pública a https://github.com/settings/keys
# Y usa: git remote add origin git@github.com:TU_USUARIO/proyecto-grupo-limpia.git
```

---

## 🌐 URLs Después de Subir

**Tu Repositorio:**
```
https://github.com/TU_USUARIO/proyecto-grupo-limpia
```

**Ver Proyecto Online (GitHub Pages):**
```
https://TU_USUARIO.github.io/proyecto-grupo-limpia
```

Para activar GitHub Pages:
1. Ve a Settings → Pages
2. Source: `main`
3. Espera 1-2 minutos

---

## 🎬 Cambios Realizados Hoy

### ✨ Optimizaciones de UI/UX:
- ✅ Botones bajados en header (padding bottom agregado)
- ✅ Espaciado sincronizado visualmente
- ✅ Responsive en mobile, tablet y desktop

### ⚡ Optimizaciones de Rendimiento:
- ✅ Videos con `preload="auto"` (carga inmediata)
- ✅ Lazy loading mejorado
- ✅ Codecs optimizados
- ✅ Threshold de intersección reducido (0.25)
- ✅ Script limpiado

### 📦 Estructura Git:
- ✅ `.gitignore` configurado
- ✅ `README.md` completado
- ✅ 3 commits con historial claro
- ✅ Listo para colaboración

---

## 💡 Próximos Pasos (Opcional)

```bash
# Ver estado actual
git status

# Ver historial de commits
git log --oneline

# Agregar cambios nuevos
git add .
git commit -m "Descripción del cambio"
git push

# Crear branch para nuevas features
git checkout -b feature/mi-nueva-caracteristica
git push origin feature/mi-nueva-caracteristica
```

---

**¿Necesitas ayuda?** Comparte tu usuario de GitHub y te doy el comando exacto para ejecutar.
