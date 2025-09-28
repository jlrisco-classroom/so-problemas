# Repositorio de Problemas de la Asignatura de Sistemas Operativos

Bienvenidos al repositorio colaborativo para la resolución de problemas de la asignatura de Sistemas Operativos.

## Objetivo

Este espacio tiene un doble propósito:

1.  **Construir una base de conocimiento colectiva** donde resolvamos y discutamos los problemas teóricos y prácticos de la asignatura.
2.  **Proporcionar experiencia práctica** con Git y GitHub, herramientas esenciales en el mundo del desarrollo de software, siguiendo un flujo de trabajo profesional basado en Ramas y *Pull Requests*.

## Organización del Repositorio

Para mantener la claridad y el orden, los problemas están organizados por temas dentro de la carpeta `soluciones/`. La nomenclatura de los archivos es la siguiente:

`soluciones/problema-2.1.md`

Este nombre representa el **primer problema** de la hoja de ejercicios correspondiente al **tema 2**. Todos los ficheros utilizarán la extensión `.md` (Markdown).

## Flujo de Trabajo

Para evitar conflictos y asegurar que la colaboración sea ordenada, **no trabajaremos directamente sobre la rama `main`**. Seguiremos un flujo de trabajo estándar en la industria:

**1. Sincroniza tu Repositorio Local**
Antes de empezar a trabajar, asegúrate de tener la última versión de la rama `main`:

```bash
git checkout main
git pull origin main
```

**2. Elige un Problema y Crea una Rama**
Busca un problema que no esté resuelto en la sección de **"Issues"** de GitHub. Si nadie está asignado, puedes empezar a trabajar en él. Crea una nueva rama para tu solución desde `main`:

```bash
# Formato: solucion/TEMA.PROBLEMA/tu-usuario-github
git checkout -b solucion/2.1/juan-perez
```

**3. Resuelve el Problema**
Crea el archivo Markdown en la carpeta correspondiente (ej: `soluciones/problema-2.1.md`). Consulta la **"Guía para una Buena Solución"** más abajo para saber qué esperamos de tu respuesta.

**4. Guarda tus Cambios (Commit)**
Una vez estés satisfecho con tu solución, haz commit de tus cambios. Usa un mensaje de commit claro y descriptivo.

```bash
git add soluciones/problema-2.1.md
git commit -m "Resuelve el problema 2.1 sobre el modelo de ficheros POSIX"
```

**5. Sube tu Rama a GitHub**
Ahora, sube tu rama al repositorio remoto:

```bash
git push origin solucion/2.1/juan-perez
```

**6. Abre un *Pull Request* (PR)**
Ve a la página del repositorio en GitHub. Verás una notificación para crear un **Pull Request** desde tu nueva rama. Ábrelo, añade una breve descripción y enlaza la *Issue* que resuelve.

**7. Discusión y Revisión en Clase**
Tu *Pull Request* será el que **proyectaremos y discutiremos en clase**. Es una propuesta de solución. El resto de compañeros y el profesor podrán hacer comentarios, sugerir cambios y resolver dudas directamente sobre tu PR. Si hay que hacer cambios, solo tienes que hacer nuevos *commits* en tu rama y el PR se actualizará solo.

**8. Fusión de la Solución**
Una vez la solución se considere correcta y definitiva por parte de la clase, el profesor la **fusionará (`merge`)** con la rama `main`. Tu aportación pasará a ser parte de la solución oficial de la asignatura.

## Guía para una Buena Solución

Una solución de calidad es la que no solo es correcta, sino también didáctica. Debe incluir:

  * **Contexto Teórico:** Una breve introducción explicando qué conceptos de la asignatura aplican al problema (p. ej., "Este problema sobre `fork()` y `exec()` se relaciona con la creación de procesos y la carga de programas vista en el tema 3").

  * **Desarrollo y Explicación:** La lógica y los pasos seguidos para llegar a la solución. Si es un problema de código, explica las decisiones clave.

  * **Código Formateado:** Utiliza bloques de código Markdown con resaltado de sintaxis. Es fundamental para la legibilidad.

    **Ejemplo para código C:**

    ````markdown
    ```c
    #include <stdio.h>

    int main() {
        printf("Hola, SO!\n");
        return 0;
    }
    ```
    ````

    **Ejemplo para comandos de terminal:**

    ````markdown
    ```bash
    ls -l | grep ".c"
    ```
    ````

  * **Resultado Final:** Muestra la salida del programa o la respuesta final al problema de forma clara.

## Formato de Archivos: Markdown

Para mantener la consistencia y facilitar la revisión en la web de GitHub, todos los problemas se resolverán en formato **Markdown (`.md`)**. Este formato es sencillo, potente y perfectamente integrado en el ecosistema de desarrollo actual.

## Discusión y Colaboración

Los *Pull Requests* son nuestro espacio principal para el debate. Si dos estudiantes proponen soluciones diferentes para el mismo problema, se pueden abrir dos PRs y la discusión en clase servirá para comparar ambos enfoques y decidir cuál es el más adecuado antes de fusionar nada. El objetivo es llegar a un consenso a través del diálogo técnico.

Gracias a todos por vuestra colaboración.
