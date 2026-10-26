# Flujo Colaborativo

Esta guía documenta el proceso estándar para trabajar con repositorios remotos, hacer *forks* y proponer cambios de manera segura utilizando Git y GitHub.

## Conceptos Fundamentales

Antes de empezar a codificar, es importante entender cómo interactúan nuestros repositorios:

*   **Fork:** Una copia personal del repositorio de otra persona en tu propia cuenta de GitHub.
*   **Clone:** La acción de descargar un repositorio remoto (como tu fork) a tu computadora local.
*   **Pull Request (PR):** Una petición formal para que los dueños del proyecto original revisen e integren tus cambios.
*   **Origin:** El apodo por defecto que Git le da al repositorio remoto del cual clonaste el proyecto.

## Flujo de Trabajo Paso a Paso

Sigue este procedimiento para contribuir al proyecto sin afectar la rama principal (`main`):

1. Sincroniza tu repositorio local trayendo las últimas novedades del original.
2. Crea una nueva rama descriptiva para tu corrección o característica.
3. Realiza los cambios en el código (por ejemplo, corregir la función `calcularTotal` en `script.js`).
4. Añade y confirma los cambios con un mensaje claro.
5. Sube tu rama al repositorio remoto y abre un *Pull Request*.

### Lista de Tareas del Laboratorio

Para llevar un control de tu progreso, marca las siguientes casillas conforme avances:

- [x] Hacer un fork del repositorio ajeno.
- [x] Clonar el fork en la computadora local.
- [x] Reportar un error mediante un Issue claro y verificable.
- [ ] Corregir el error en una rama propia (`fix-total-carrito`).
- [ ] Proponer el cambio abriendo un Pull Request.

### Comandos Principales de Git

En la siguiente tabla se describen los comandos más utilizados durante este flujo de trabajo:

| Comando Git | Descripción |
| :--- | :--- |
| `git clone <url>` | Descarga una copia exacta del repositorio remoto a tu equipo. |
| `git checkout -b <rama>` | Crea una rama nueva y se cambia a ella inmediatamente. |
| `git diff` | Muestra las diferencias exactas de código antes de confirmarlas. |
| `git push origin <rama>` | Sube la rama local con tus commits a tu repositorio remoto (fork). |

### Ejemplo Práctico de Commit

Cuando estés listo para guardar tus cambios, asegúrate de referenciar el número de *Issue* si estás corrigiendo un problema. Aquí tienes un ejemplo de cómo hacerlo en la terminal:

```bash
git add script.js
git commit -m "Corrige el calculo del total del carrito (#363)"
```

---

![Esquema de flujo de ramas en Git](https://docs.github.com/assets/images/help/repository/branching.png)