# 🛠️ Comandos Git

## ⚙️ **Configurar Git**

1. Configura tu nombre de usuario y correo electrónico en Git (si aún no lo has hecho):

   ```bash
   git config --global user.name "Tu Nombre"
   git config --global user.email "tuemail@example.com"
   git config --global core.autocrlf true
   ```

---

## 📦 **Clonar un repositorio**

Clona el repositorio desde GitHub usando el siguiente comando:

```bash
gh repo clone kyozApp/comandosGit
```

---

## 🧩 **Inicializar un repositorio y configurar la rama principal**

2. Inicializa un nuevo repositorio Git:

   ```bash
   git init
   ```

3. Cambia el nombre de la rama principal a `main`:

   ```bash
   git branch -m master main
   ```

---

## 📂 **Añadir y confirmar cambios**

4. Añade todos los archivos al área de preparación:

   ```bash
   git add .
   ```

5. Realiza un commit con un mensaje descriptivo:

   ```bash
   git commit -m "Mensaje de commit"
   ```

---

## 🚀 **Crear y subir a GitHub**

6. Crea un repositorio en GitHub utilizando la CLI de GitHub:

   - Para un repositorio público:

     ```bash
     gh repo create comandosGit --public --source=.
     ```

   - Para un repositorio privado:

     ```bash
     gh repo create comandosGit --private --source=.
     ```

7. Sube los cambios al repositorio remoto:

   ```bash
   git push -u origin main
   ```

---

## 🔍 **Gestión de ramas**

- Ver las ramas locales:

  ```bash
  git branch
  ```

- Ver todas las ramas (locales y remotas):

  ```bash
  git branch -a
  ```

- Crear una nueva rama basada en otra rama remota:

  ```bash
  git checkout -b nombre-de-la-rama origin/nombre-de-la-rama # Por ejemplo git checkout -b Erick origin/Erick
  ```

---

## 🔄 **Sincronización con el repositorio remoto**

- Actualizar el repositorio local con los cambios de la rama `main`:

  ```bash
  git pull origin main
  ```

- Subir cambios de una rama local a `main`:

  ```bash
  git push origin nombre-de-la-rama:main
  ```

---

### ✅ **Notas finales**
- Usa estos comandos para mantener tu flujo de trabajo organizado y sincronizado con el repositorio remoto.
- Recuerda siempre verificar los cambios antes de hacer un `commit` o `push`.

