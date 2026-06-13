# 🛠️ TuleApp QA Workflow & Management

Este repositorio centraliza la gobernanza, planificación de pruebas, matrices de trazabilidad y metodologías ágiles aplicadas al ecosistema de software.

## 📋 Contenido del Repositorio
* **`/templates`**: Plantillas estandarizadas para reportes de bugs y casos de prueba.
* **`Matrix-Trazabilidad.md`**: Mapeo directo entre requerimientos y código automatizado de Cypress.

## 🖼️ Flujo de Gestión de Calidad (Tablero Agile)
Aquí se muestra el flujo de trabajo del ciclo de vida de los defectos e historias de usuario mapeados en el proyecto:

![Tablero de Gestión]<img width="1301" height="434" alt="tablero-kanban" src="https://github.com/user-attachments/assets/313b7b81-b850-4676-8b4e-a37a42ba04c7" />
*(Nota para Daniel: Reemplaza esta imagen por una captura de pantalla real de un tablero Kanban que simules en GitHub Projects o TuleApp con columnas: To Do, In Progress, QA Testing, Done)*.

## 🔗 Conexión al Ecosistema CI/CD
1. Los casos de prueba aquí definidos se encuentran automatizados en: [cypress-e2e-suite](https://github.com/Danielito2252/cypress-e2e-suite)[cite: 1].
2. Los reportes de ejecución se inyectan directamente mediante el pipeline alojado en: [Jenkins-Devsecops-Pipeline](https://github.com/Danielito2252/Jenkins-Devsecops-Pipeline)[cite: 1].

## 📄 Licencia
Este proyecto está bajo la licencia MIT.