# 📤 Cómo publicar este README en tu perfil de GitHub

GitHub usa un repositorio especial llamado **igual que tu usuario** (`azulls1/azulls1`) cuyo `README.md` se muestra en tu perfil público.

## Opción A — Crear el repo desde la web (más fácil)

1. Ve a https://github.com/new
2. **Repository name**: `azulls1` ← exactamente igual que tu usuario
3. Marca **Public**
4. Marca **Add a README file** (lo sobrescribiremos después)
5. Click **Create repository**
6. En el repo recién creado, sube los archivos de esta carpeta:
   - `README.md`
   - `.github/workflows/snake.yml`

Puedes arrastrar y soltar desde el explorador de Windows en la página del repo (botón **Add file → Upload files**).

## Opción B — Desde la línea de comandos (Git)

Asegúrate de tener `git` instalado y autenticado con GitHub. Desde PowerShell, parado en esta carpeta:

```powershell
cd "C:\Users\shernandez\Documents\azulls1-profile"

git init -b main
git add .
git commit -m "feat: modern GitHub profile README"
git remote add origin https://github.com/azulls1/azulls1.git
git push -u origin main
```

> Si nunca lo creaste, primero ve a https://github.com/new y crea el repo `azulls1` (público, **sin** README ni .gitignore), luego ejecuta los comandos.

## Activar la animación de la serpiente 🐍

Una vez subido el repo:

1. En GitHub, ve a tu repo `azulls1/azulls1`.
2. Pestaña **Actions** → si pide habilitarlas, acepta.
3. Verás un workflow llamado **Generate Snake Animation**.
4. Click en él → botón **Run workflow** → confirma.
5. Espera ~1 min. Se generará una rama `output` con los SVGs.
6. Recarga tu perfil https://github.com/azulls1 — la serpiente aparecerá.

A partir de ahí se regenera sola cada 12 horas y cada vez que hagas push a `main`.

## Personalización rápida

Cosas que puedes ajustar en `README.md`:

- **Foto**: cambia `avatars.githubusercontent.com/azulls1` por una URL personalizada.
- **Frases del typing**: línea con `&lines=...` → separa con `;` los textos a rotar.
- **Tema de stats**: cambia `theme=tokyonight` por `radical`, `dracula`, `gruvbox`, `synthwave`, etc.
- **Colores**: `00D9FF` es el accent; busca y reemplaza por tu color favorito.

## Tip pro: pinea repos personales

En tu perfil → **Customize your pins** → elige 6 repos tuyos para destacar (puedes mantener los actuales o subir nuevos personales).
