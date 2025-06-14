Proyecto web básico para demostrar el flujo de trabajo con Git y GitHub.
# Wiki de Overwatch - Proyecto Colaborativo

Este repositorio contiene el código fuente de una mini-wiki sobre el universo de Overwatch, creada como una demostración práctica de un flujo de trabajo colaborativo utilizando Git y GitHub.

## 🎯 Objetivo del Proyecto

El objetivo principal es construir una página web funcional y atractiva que sirva como una pequeña base de datos sobre héroes, mapas o habilidades de Overwatch. A través de su desarrollo, buscamos aplicar y documentar un ciclo de trabajo profesional que incluye el manejo de ramas, la revisión de código mediante Pull Requests y la gestión de calidad antes de integrar cualquier cambio a la versión final.

---

## 👥 Integrantes y Roles

| Rol | Integrante |
| :--- | :--- |
| 👑 **Líder** | David Rodriguez |
| 🏗️ **Integrador** | Raymundo Rivera |
| 🎨 **Diseñador** | Mario Mejía |
| 📝 **Documentador**| Celeste Becerra |
| 🕵️ **Tester / QA** | Saul Flores |

---

## 🛠️ Flujo de Trabajo Usado (Git Flow Simplificado)

Para garantizar un desarrollo ordenado y de alta calidad, nuestro equipo ha implementado un flujo de trabajo basado en ramas, siguiendo estos principios:

1.  **Rama `main`**:
    * Es nuestra rama principal y representa la versión estable y pública de la wiki.
    * Está protegida: Nadie puede subir cambios directamente. Todo debe pasar por un Pull Request.

2.  **Ramas de Desarrollo Principales**:
    * Hemos definido dos ramas de desarrollo continuas, cada una asignada a un rol clave:
        * **`dev-html`**: Rama utilizada por el **Integrador (Raymundo Rivera)** para construir y modificar toda la estructura HTML de la wiki.
        * **`dev-css`**: Rama utilizada por el **Diseñador (Mario Mejía)** para trabajar en los aspectos visuales y de estilo (CSS).
    * Para otras tareas, como actualizar esta documentación, se crean ramas temporales (ej: `docs`).

3.  **Pull Requests (PRs)**:
    * Una vez que se completa una tarea en `dev-html` o `dev-css`, se abre un Pull Request para proponer la fusión de esos cambios hacia la rama `main`.
    * En el PR se describe qué cambios se hicieron y por qué.

4.  **Revisión de Código y Control de Calidad**:
    * Cada PR debe ser revisado y aprobado por al menos dos personas:
        * El **Tester / QA (Saul Flores)**, quien verifica que los cambios no introduzcan errores y funcionen como se espera.
        * El **Líder (David Rodriguez)**, quien realiza la revisión final y aprueba la fusión.
    * Solo después de recibir ambas aprobaciones, los cambios son integrados a `main`.

5.  **Resolución de Conflictos**:
    * Si surgen conflictos de código, estos se resuelven en la rama de desarrollo (`dev-html` o `dev-css`) antes de que el Pull Request pueda ser fusionado, manteniendo la rama `main` siempre limpia y funcional.
