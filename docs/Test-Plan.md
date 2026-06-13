# 📋 Plan de Pruebas Maestro (Master Test Plan) - Ecosistema CI/CD

**Proyecto:** Ecosistema Integrado de Automatización y DevSecOps  
**Versión:** 1.0.0  
**Autor:** Daniel  

---

## 1. Alcance (Scope)
Este plan de pruebas cubre la estrategia de verificación y validación para asegurar la calidad y seguridad del software antes de su despliegue a producción.

### ✔️ Incluido en las Pruebas
* **Pruebas de Interfaz de Usuario (E2E):** Flujos críticos del usuario automatizados (Login, Navegación, Flujo de compra).
* **Pruebas de API:** Verificación de contratos de servicios, códigos de respuesta HTTP y payloads.
* **Pruebas de Seguridad (DevSecOps):** Escaneo estático de código (SAST) y análisis de vulnerabilidades en dependencias (SCA).

### ❌ Excluido de las Pruebas
* Pruebas de rendimiento, carga y estrés (Performance Testing).
* Pruebas de compatibilidad con navegadores obsoletos (ej. Internet Explorer).

---

## 2. Estrategia de Pruebas e Integración
Las pruebas están diseñadas bajo un enfoque de **Shift-Left Testing**, ejecutándose de forma automatizada lo más temprano posible en el pipeline de CI/CD.

* **Nivel de Arquitectura:** Las pruebas reutilizan la lógica central definida en [Cypress-Framework](https://github.com/Danielito2252/Cypress-Framework)[cite: 1].
* **Suite de Ejecución:** Los escenarios específicos se encuentran en [cypress-e2e-suite](https://github.com/Danielito2252/cypress-e2e-suite)[cite: 1].
* **Orquestador:** Todo el ciclo es controlado por [Jenkins-Devsecops-Pipeline](https://github.com/Danielito2252/Jenkins-Devsecops-Pipeline)[cite: 1].

---

## 3. Criterios de Aceptación y Salida (Quality Gates)
Para permitir que el pipeline de Jenkins apruebe un despliegue, se deben cumplir los siguientes criterios estrictos[cite: 1]:

| Métrica de Calidad | Criterio de Aceptación | Herramienta |
| :--- | :--- | :--- |
| **Pruebas E2E Funcionales** | 100% Exitosas (0 Fallos) | Cypress[cite: 1] |
| **Pruebas de API** | 100% Exitosas (0 Fallos) | Cypress[cite: 1] |
| **Vulnerabilidades de Código** | 0 Críticas / 0 Altas (Quality Gate OK) | SonarQube[cite: 1] |
| **Seguridad de Contenedores** | 0 Vulnerabilidades bloqueantes | Trivy / SCA[cite: 1] |