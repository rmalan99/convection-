## Personal **Git Conventions Frontend**

En este documento se detalla un flujo de trabajo matenible y seguible.

---

*   Naming Conventions
    *   Branches
    *   Commits
*   Workflow
    *   Setup
    *   Development
    *   Release
    *   Versioning

## Naming Conventions

Convenciones en la nomenclatura para ramas y mensajes de commit.

### **👉Ramas**

 Para las ramas, usaremos la estructura `<token>/<short-descriptive-name>` o  `<code>-<token>/<location><short-descriptive-name>`

    Los `<code>` hacen referencia al tickets o tarea proveniente de gestor.  `<jira-01 || jira01>-<token>/<location><short-descriptive-name>`

    Las `<location>` Lugar donde se testa trabajando. `<code>-<token>/<authmodule || auth-module><short-descriptive-name>`

    Las `<short-descriptive-name>`  descripcion breve de que devil 👿 se esta haciendo . `<code>-<token>/<location><fix-styles>`

 Los `<token>` que podemos usar son:

*   **depen**: mejoras en temas de administración/mantenimiento del proyecto (i.e. actualización de dependencias).
*   `**docs**`: creación/actualización de documentación (i.e.: guía de configuración del proyecto).
*   `**feature**`: nuevas funcionalidades que serán incluidas en el proyecto. (i.e. visualización de cursos).
*   `**fix**`/**bugfix**/`**patch**`: corrección de un bug esperado o inesperado (i.e. links rotos).
*   `**hotfix**`: corrección de un bug inesperado y que su correccion es proritario⚡.
*   `**refactor**`: mejoras/reescritura de features existentes, no agrega un cambio grande a lo que actualmente tiene. (i.e. cambiar estados locales usando stateless components conectados a Redux).
*   `**test**`: agrega tests a un feature existente que no cuenta con los mismos (i.e. unit testing del componente de login).
*   **styles**: cambios de styles o ajuste de css styles en uno o mas componetes (i.e. styles del componente de login).
*   **grammar**: cambios grammatical.
*   **temp**: temporal changes o checkpoint changes nota: testas Ramas deben ser eliminadas luego de sierto tiempo prudente 

     `<code>-<test>/<location><short-descriptive-name>`

---

  Nota: Se podría evitar el uso de conectores :thinking\_face: 

  thinking\_face❌

  thinking-face✅

---

### **🖕Commits**

    En resumen, la estructura de los mensajes de commit es  `<type>:<subject>` o `<type>(<scope>): <subject>`.

   El `(<scope>)` Lugar donde se realiza el cambio .

   El `<subject>` mesage que descrive lo realized .

   El `<type>` son tokens cortos similares a los de las ramas, pueden ser: `style`, `refactor`, `test` , `chore`.

*   **depen**: mejoras en temas de administración/mantenimiento del proyecto (i.e. actualización de dependencias).
*   `**docs**`: creación/actualización de documentación (i.e.: guía de configuración del proyecto).
*   `**feature**`: nuevas funcionalidades que serán incluidas en el proyecto. (i.e. visualización de cursos).
*   `**fix**`/**bugfix**/`**patch**`: corrección de un bug esperado o inesperado (i.e. links rotos).
*   `**hotfix**`: corrección de un bug inesperado y que su correccion es proritario⚡.
*   `**refactor**`: mejoras/reescritura de features existentes, no agrega un cambio grande a lo que actualmente tiene. (i.e. cambiar estados locales usando stateless components conectados a Redux).
*   `**test**`: agrega tests a un feature existente que no cuenta con los mismos (i.e. unit testing del componente de login).
*   **styles**: cambios de styles o ajuste de css styles en uno o mas componetes (i.e. styles del componente de login).
*   **grammar**: cambios grammatical.

   El `scope` hace referencia al lugar en donde se han trabajado los cambios.

   El `subject` debe cumplir algunas reglas más específicas:

*   En inglés, usar modo imperativo, present tense: **change** en vez de _changed_ o _changes_.
*   La primera letra en mayúsculas (para seguir el estándar por defecto que usa Git al hacer un `merge` o `rebase`).
*   Intentar acortar el mensaje a 50 caracteres, no debe pasar de 78.
*   No poner punto al final

> Nota: Los mensajes de commits no describen lo que alguien del equipo ha trabajado, por el contrario debe describir a la persona que obtendrá o aplicará los commits, lo que el pasará proyecto.
> 
> Ejemplo:
> 
> *   _~I~_ "Added Github field in profile settings" ✗
> *   _~Someone~_ "Adds Github field in profile settings" ✗
> *   _~This commit will~_ "Add Github field to profile settings" ✔

### 🌼Branch Life

La ramas debe ser eliminadas luego de su merge a main branch 🌿  
Las ramas con el \<token> temp(temp/fix-styles) deben ser eliminadas luego de un tiempo prudente  
 

### 🐶GitHub Repository

Mantener solo las ramas necesarias, tomar en cuenta [branch life](#Branch life)
