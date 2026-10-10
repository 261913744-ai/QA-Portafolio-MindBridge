# 🧪 MindBridge - QA Strategy & Execution Project

![Status](https://img.shields.io/badge/Status-Completed-success)
![Role](https://img.shields.io/badge/Role-QA_Engineer-blue)

## 📌 Descripción del Proyecto
Este repositorio contiene la documentación formal del ciclo de pruebas de calidad (**STLC**) realizado para la funcionalidad **"Shareable Content"** de la plataforma educativa **MindBridge**.

El objetivo del proyecto fue garantizar la estabilidad del software, definir responsabilidades entre equipos, escribir criterios de aceptación bajo metodología **BDD** e identificar defectos críticos en el backend en un entorno de *Staging*.

---

## 🛠️ Herramientas y Tecnologías
* **Gestión de Pruebas:** Jira (User Stories, Backlog y BDD).
* **Metodología de Pruebas:** BDD (*Behavior-Driven Development* con sintaxis Gherkin).
* **Inspección de Red / API:** Chrome DevTools (Network tab, HTTP Status Codes).
* **Técnicas Aplicadas:** 
  * *Static Testing:* Revisión de requerimientos y Pull Requests.
  * *Dynamic Testing:* Pruebas exploratorias, funcionales, de API y diseño responsivo (*Mobile Viewport*).
* **Entorno de Pruebas:** Staging (`http://localhost:3000`).

---

## 🚀 Entregables y Estructura del Documento

### 1. Arquitectura y Matriz RACI
Se estableció la distribución de responsabilidades para las tres capas del sistema (**UI, API, DB**) asignando roles claros entre el equipo de QA y Desarrollo.

### 2. Criterios de Aceptación (BDD - Given/When/Then)
Se redactaron 3 escenarios probados y documentados en Jira:
* **Scenario 1 (Happy Path):** Generación exitosa de enlace de compartir con nota personalizada.
* **Scenario 2 (Edge Case):** Validación de la interfaz en pantallas móviles pequeñas (*iPhone SE / < 375px*).
* **Scenario 3 (Error Condition):** Manejo de validaciones al enviar notas vacías.

### 3. Reporte de Defecto (DEF-001)
* **Fallo Encontrado:** Respuesta `HTTP 500 Internal Server Error` al generar un enlace con nota vacía.
* **Severidad / Prioridad:** Alta / Alta.
* **Impacto:** Bloqueo de la experiencia de usuario debido a falta de validación en el frontend/backend.
* **Evidencia:** Captura de pantalla del fallo en la UI e inspección directa del fallo en la pestaña *Network* de DevTools.

---

## 📄 Archivo Adjunto
Puedes consultar el reporte formal completo en formato PDF cargado en este repositorio:
* 📥 **[Ver / Descargar QA Strategy and Execution Document](./QA%20Strategy%20and%20Execution%20Templ.pdf)**

---

👤 **Autor:** Jonathan Rogelio Galindo Veltran  
📅 **Fecha:** Octubre 2026
