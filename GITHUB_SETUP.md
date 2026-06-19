# Pasos para Conectar con GitHub

## ✅ Configuración Local Completada

Tu proyecto ya está inicializado con Git y listo para subir a GitHub. El commit inicial ha sido creado correctamente:

```
38711a9 - Initial commit: Proyecto Grupo Limpia - Sitio web de limpieza corporativa premium
```

## 📋 Pasos para Subir a GitHub

### 1. Crear Repositorio en GitHub

1. Ve a [github.com/new](https://github.com/new)
2. **Repository name:** `proyecto-grupo-limpia`
3. **Description:** Sitio web de limpieza corporativa premium en Cartagena
4. **Public** (para que todos puedan verlo)
5. ⚠️ **NO selecciones** "Initialize this repository with"
6. Haz clic en **"Create repository"**

### 2. Conectar tu Repositorio Local

Una vez creado, GitHub te mostrará un comando. Copia y ejecuta en tu terminal:

```bash
cd /home/riano200612/proyecto-grupo-limpia

# Renombrar rama a 'main' (recomendado)
git branch -M main

# Conectar con GitHub (reemplaza TU_USUARIO con tu usuario de GitHub)
git remote add origin https://github.com/TU_USUARIO/proyecto-grupo-limpia.git

# Hacer push del código
git push -u origin main
```

### 3. Autenticación

GitHub te pedirá autenticación. Tienes dos opciones:

#### Opción A: Token de Acceso Personal (Recomendado)

1. Ve a [github.com/settings/tokens](https://github.com/settings/tokens/new)
2. Crea un **Personal Access Token** con permisos `repo`
3. Copia el token
4. Cuando Git te pida contraseña, pega el token

#### Opción B: SSH (Alternativa)

```bash
# Generar clave SSH
ssh-keygen -t ed25519 -C "tu-email@example.com"

# Agregar la clave pública a GitHub
cat ~/.ssh/id_ed25519.pub

# Copiar la salida a https://github.com/settings/keys

# Usar URL SSH en lugar de HTTPS
git remote add origin git@github.com:TU_USUARIO/proyecto-grupo-limpia.git
```

---

## 🚀 Comandos Git Útiles

Después de conectar con GitHub, usa estos comandos:

```bash
# Ver estado de cambios
git status

# Agregar cambios
git add .

# Hacer commit
git commit -m "Descripción del cambio"

# Subir cambios a GitHub
git push

# Descargar cambios del servidor
git pull

# Ver historial
git log --oneline
```

---

## 📂 Estructura del Proyecto

```
proyecto-grupo-limpia/
├── .git/                  # Carpeta Git (no tocar)
├── .gitignore             # Archivos a ignorar
├── README.md              # Documentación
├── index.html             # Página principal
└── assets/
    └── imagenes/
        ├── VIDEO_HOGAR_FELIZ.mp4
        ├── VIDEO_COCINA_INDUSTRIAL.mp4
        ├── VIDEO_CORPORATIVO_PREMIUM_PARA.mp4
        └── logo-grupo-limpia.png
```

---

## ✨ Próximos Pasos

Después de subir a GitHub:

1. **Habilitar GitHub Pages** (para hosting gratuito)
   - Ve a Settings → Pages
   - Source: Branch `main`
   - Tu sitio estará en: `https://TU_USUARIO.github.io/proyecto-grupo-limpia`

2. **Agregar descripción** al repositorio

3. **Crear releases** cuando hagas actualizaciones importantes

4. **Usar branches** para desarrollo:
   ```bash
   git checkout -b feature/nueva-seccion
   git commit -m "Agregar nueva sección"
   git push origin feature/nueva-seccion
   ```

---

**¿Necesitas ayuda?** Responde con tu usuario de GitHub y te ayudaré a completar el proceso.
