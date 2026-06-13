# 📊 Matriz de Trazabilidad de Requisitos (RTM)

Esta matriz conecta los requisitos de negocio descritos en la gestión del proyecto con los scripts de prueba automatizados en Cypress.

| ID Requisito | Descripción del Requisito | ID Ticket | Estado QA | Script Automatizado (Cypress) |
| :--- | :--- | :--- | :--- | :--- |
| **REQ-001** | El usuario debe poder iniciar sesión de forma segura. | #101 | 🟩 PASSED | [login.cy.ts (Repo 1)](https://github.com/Danielito2252/cypress-e2e-suite) |
| **REQ-002** | El sistema debe rechazar inyecciones SQL en el login. | #102 | 🟩 PASSED | [security-api.cy.ts (Repo 1)](https://github.com/Danielito2252/cypress-e2e-suite) |
| **REQ-003** | El pipeline debe detenerse si hay vulnerabilidades críticas. | #103 | 🟩 PASSED | [Jenkinsfile (Repo 2)](https://github.com/Danielito2252/Jenkins-Devsecops-Pipeline) |