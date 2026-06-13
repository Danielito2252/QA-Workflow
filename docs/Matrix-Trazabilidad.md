# 📊 Matriz de Trazabilidad de Requisitos (RTM)

Esta matriz garantiza que cada funcionalidad requerida por el negocio esté respaldada por una prueba automatizada en el repositorio de Cypress y validada por el pipeline de Jenkins[cite: 1].

| ID Requisito | Requisito de Software | ID Ticket (Kanban) | Estado QA | Script de Prueba Automatizada | Etapa del Pipeline Validadora |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **REQ-01** | El usuario debe poder iniciar sesión con credenciales válidas[cite: 1]. | `TSK-01` | 🟩 PASSED | [`login.cy.ts` (Repo 1)](https://github.com/Danielito2252/cypress-e2e-suite) | `E2E Functional Tests`[cite: 1] |
| **REQ-02** | La aplicación debe rechazar inicios de sesión con formatos inválidos. | `TSK-03` | 🟩 PASSED | [`login-api.cy.ts` (Repo 1)](https://github.com/Danielito2252/cypress-e2e-suite) | `API Testing`[cite: 1] |
| **REQ-03** | El código fuente no debe contener vulnerabilidades críticas inyectadas. | `BUG-102` | 🟩 PASSED | N/A (Análisis Estático) | `SAST Scan (SonarQube)`[cite: 1] |
| **REQ-04** | Las dependencias de software y librerías deben estar libres de exploits conocidos. | `TSK-04` | 🟩 PASSED | N/A (Análisis de Librerías) | `SCA Scan (Trivy)`[cite: 1] |