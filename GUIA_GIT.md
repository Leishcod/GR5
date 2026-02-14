# Guía Rápida de Git: Proyectos y Comandos Diarios

Esta guía te ayuda a manejar tu código con Git y GitHub.

## 1. Comandos Diarios (En tu proyecto actual)

Cada vez que haces cambios y quieres guardarlos en la nube, usa estos 3 comandos en orden:

1.  **Guardar los cambios (Stage):**
    ```powershell
    git add .
    ```

2.  **Confirmar los cambios (Commit):**
    ```powershell
    git commit -m "Escribe aquí qué cambios hiciste"
    ```
    *(Ejemplo: `git commit -m "Agregue nuevos estilos al banner"`) - Las comillas son importantes.*

3.  **Subir a GitHub (Push):**
    ```powershell
    git push
    ```

---

## 2. ¿Qué pasa si cambio de proyecto (carpeta)?

Git funciona **por carpeta**. Si vas a trabajar en OTRO proyecto:

1.  **Abre la terminal en la NUEVA carpeta** del otro proyecto.
2.  Si es un proyecto **NUEVO** (que nunca has subido):
    *   Ejecuta `git init`.
    *   Crea un **NUEVO** repositorio vacío en GitHub.
    *   Sigue los mismos pasos de conexión (`git remote add...`, etc.).
3.  Si es un proyecto **YA EXISTENTE** (que ya tiene Git):
    *   Solo usa `git pull` (para bajar cambios) o `git push` (para subir), igual que siempre.

**IMPORTANTE:** Nunca trates de mezclar proyectos. Cada carpeta de proyecto tiene su propio `.git` oculto que sabe a dónde pertenece.

---

## 3. ¿A qué proyecto de GitHub estoy conectado?

Si alguna vez tienes duda de a qué repositorio está conectada tu carpeta actual, ejecuta:

```powershell
git remote -v
```

Esto te mostrará la URL del repositorio remoto (GitHub) al que estás subiendo tus cambios.
