# 🧪 CASO DE PRUEBA: TC-[ID] - [Nombre del caso]

**Prioridad:** Alta / Media / Baja  
**Requisito del Sistema:** REQ-01 - Autenticación de Usuarios  
**Automatizado:** Sí (Cypress)

## ⚙️ Precondiciones
* El usuario debe estar registrado.
* La base de datos debe estar limpia en el entorno de QA.

## 🛤️ Pasos de la Prueba
1. Ingresar a la URL de la aplicación.
2. Digitar credenciales válidas.
3. Hacer clic en "Login".

## 🎯 Resultado Esperado
El sistema redirige al Dashboard y muestra el token de sesión.

## 🔗 Código de Automatización
* **Script de Cypress:** [Ver archivo de prueba en Repo 1](https://github.com/Danielito2252/cypress-e2e-suite/blob/main/cypress/e2e/login.cy.ts)