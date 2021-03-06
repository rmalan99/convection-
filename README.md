## Version Do **Git Conventions Frontend**

En este documento se detalla el flujo de trabajo que seguimos (seguiremos) en el equipo de desarrollo del LMS.

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

### **馃憠Ramas**

 Para las ramas, usaremos la estructura `<token>/<short-descriptive-name>` o 聽`<code>-<token>/<location><short-descriptive-name>`

聽 聽 Los `<code>` hacen referencia al tickets o tarea proveniente de gestor. 聽`<jira-01 || jira01>-<token>/<location><short-descriptive-name>`

聽 聽 Las `<location>` Lugar donde se testa trabajando. `<code>-<token>/<authmodule || auth-module><short-descriptive-name>`

聽 聽 Las `<short-descriptive-name>` 聽descripcion breve de que devil 馃懣 se esta haciendo . `<code>-<token>/<location><fix-styles>`

 Los `<token>` que podemos usar son:

*   **depen**: mejoras en temas de administraci贸n/mantenimiento del proyecto (i.e. actualizaci贸n de dependencias).
*   `**docs**`: creaci贸n/actualizaci贸n de documentaci贸n (i.e.: gu铆a de configuraci贸n del proyecto).
*   `**feature**`: nuevas funcionalidades que ser谩n incluidas en el proyecto. (i.e. visualizaci贸n de cursos).
*   `**fix**`/**bugfix**/`**patch**`: correcci贸n de un bug esperado o inesperado (i.e. links rotos).
*   `**hotfix**`: correcci贸n de un bug inesperado y que su correccion es proritario鈿?.
*   `**refactor**`: mejoras/reescritura de features existentes, no agrega un cambio grande a lo que actualmente tiene. (i.e. cambiar estados locales usando stateless components conectados a Redux).
*   `**test**`: agrega tests a un feature existente que no cuenta con los mismos (i.e. unit testing del componente de login).
*   **styles**: cambios de styles o ajuste de css styles en uno o mas componetes (i.e. styles del componente de login).
*   **grammar**: cambios grammatical.
*   **temp**: temporal changes o checkpoint changes nota: testas Ramas deben ser eliminadas luego de sierto tiempo prudente聽

聽 聽 聽`<code>-<test>/<location><short-descriptive-name>`

---

聽 Nota: Se podr铆a evitar el uso de conectores :thinking\_face:聽

聽 thinking\_face鉂?

聽 thinking-face鉁?

---

### **馃枙Commits**

聽 聽 En resumen, la estructura de los mensajes de commit es 聽`<type>:<subject>` o `<type>(<scope>): <subject>`.

聽 聽El `(<scope>)` Lugar donde se realiza el cambio .

聽 聽El `<subject>` mesage que descrive lo realized .

聽 聽El `<type>` son tokens cortos similares a los de las ramas, pueden ser: `style`, `refactor`, `test` , `chore`.

*   **depen**: mejoras en temas de administraci贸n/mantenimiento del proyecto (i.e. actualizaci贸n de dependencias).
*   `**docs**`: creaci贸n/actualizaci贸n de documentaci贸n (i.e.: gu铆a de configuraci贸n del proyecto).
*   `**feature**`: nuevas funcionalidades que ser谩n incluidas en el proyecto. (i.e. visualizaci贸n de cursos).
*   `**fix**`/**bugfix**/`**patch**`: correcci贸n de un bug esperado o inesperado (i.e. links rotos).
*   `**hotfix**`: correcci贸n de un bug inesperado y que su correccion es proritario鈿?.
*   `**refactor**`: mejoras/reescritura de features existentes, no agrega un cambio grande a lo que actualmente tiene. (i.e. cambiar estados locales usando stateless components conectados a Redux).
*   `**test**`: agrega tests a un feature existente que no cuenta con los mismos (i.e. unit testing del componente de login).
*   **styles**: cambios de styles o ajuste de css styles en uno o mas componetes (i.e. styles del componente de login).
*   **grammar**: cambios grammatical.

聽 聽El `scope` hace referencia al lugar en donde se han trabajado los cambios.

聽 聽El `subject` debe cumplir algunas reglas m谩s espec铆ficas:

*   En ingl茅s, usar modo imperativo, present tense: **change** en vez de _changed_ o _changes_.
*   La primera letra en may煤sculas (para seguir el est谩ndar por defecto que usa Git al hacer un `merge` o `rebase`).
*   Intentar acortar el mensaje a 50 caracteres, no debe pasar de 78.
*   No poner punto al final

> Nota: Los mensajes de commits no describen lo que alguien del equipo ha trabajado, por el contrario debe describir a la persona que obtendr谩 o aplicar谩 los commits, lo que el pasar谩 proyecto.
> 
> Ejemplo:
> 
> *   _~I~_ "Added Github field in profile settings" 鉁?
> *   _~Someone~_ "Adds Github field in profile settings" 鉁?
> *   _~This commit will~_ "Add Github field to profile settings" 鉁?

### 馃尲Branch Life

La ramas debe ser eliminadas luego de su merge a main branch 馃尶  
Las dramas con el \<token> temp(temp/fix-styles) deben ser eliminadas luego de un tiempo prudente  
聽

### 馃惗GitHub Repository

Mantener solo las ramas necesarias, tomar en cuenta [branch life](#Branch life)