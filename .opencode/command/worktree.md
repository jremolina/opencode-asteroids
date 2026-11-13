---
description: Crea un worktree en .worktrees/ con el nombre derivado del argumento.
---

Recibes el argumento: $ARGUMENTS

Haz exactamente lo siguiente, nada más:

1. Analiza el argumento:
   - Si tiene espacios o caracteres no válidos para una ruta (mayúsculas, símbolos, etc.), conviértelo a slug: minúsculas, guiones en lugar de espacios, sin caracteres especiales.
   - Si está vacío, deriva un nombre corto y descriptivo del contexto actual (por ejemplo, el tema o la tarea de la sesión).
2. Ejecuta EXACTAMENTE UN comando, desde el directorio actual, sin cambiar de directorio (sin `cd`):

   git worktree add .worktrees/<nombre-derivado>

3. No hagas nada más: nada de `cd`, ni otros comandos git, ni commits, ni ediciones de archivos.
4. Si los argumentos son muy largos simplificalo a algo mas significativo
