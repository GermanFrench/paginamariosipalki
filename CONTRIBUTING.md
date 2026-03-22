# Guía de Contribución

¡Bienvenido al proyecto! Esta guía explica cómo puedes contribuir al repositorio.

## ¿Por qué no puedo hacer push siendo colaborador?

Si ya fuiste agregado como colaborador pero no puedes hacer `push`, el motivo más común es que **aún no aceptaste la invitación** de GitHub.

### Pasos para solucionar el problema

1. **Acepta la invitación de GitHub**

   Busca en tu correo electrónico (incluyendo spam) un mensaje de GitHub con el asunto:
   > "GermanFrench invited you to collaborate"

   O visita directamente este enlace:
   ```
   https://github.com/GermanFrench/paginamariosipalki/invitations
   ```

2. **Verifica tu acceso**

   Después de aceptar la invitación, confirma que tienes acceso en:
   ```
   https://github.com/GermanFrench/paginamariosipalki
   ```

3. **Autentícate correctamente con Git**

   Asegúrate de estar autenticado con las credenciales correctas de GitHub al hacer push:
   ```bash
   git push origin main
   ```

   Si Git te pide usuario y contraseña, usa tu nombre de usuario de GitHub y un **token de acceso personal** (no tu contraseña). Puedes crear uno en:
   ```
   https://github.com/settings/tokens
   ```

4. **Configura SSH (opcional, recomendado)**

   Para evitar ingresar credenciales cada vez, configura SSH:
   ```bash
   ssh-keygen -t ed25519 -C "tu@email.com"
   cat ~/.ssh/id_ed25519.pub
   ```
   Copia el resultado y agrégalo en: `https://github.com/settings/keys`

   Luego cambia la URL remota a SSH:
   ```bash
   git remote set-url origin git@github.com:GermanFrench/paginamariosipalki.git
   ```

## Flujo de trabajo básico

```bash
# 1. Obtener los últimos cambios
git pull origin main

# 2. Realizar tus cambios en los archivos

# 3. Ver qué cambió
git status

# 4. Agregar los cambios
git add .

# 5. Hacer commit con un mensaje descriptivo
git commit -m "Descripción de los cambios"

# 6. Subir los cambios
git push origin main
```

## ¿Necesitas ayuda?

Si sigues teniendo problemas, contacta al dueño del repositorio para verificar que tu cuenta de GitHub tiene los permisos correctos.
