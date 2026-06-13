---
name: "🧪 Test Case"
about: Diseñar un nuevo caso de prueba manual o automatizado para el ciclo de vida del software.
title: "[TC] "
labels: test-case, automation-candidate
assignees: ''
---

## 🆔 Identificador del Caso de Prueba
**TC-00X** - [Nombre descriptivo de la prueba]

## 🎯 Objetivo y Precondiciones
* **Objetivo:** Verificar que [funcionalidad] responda correctamente bajo las condiciones de negocio.
* **Precondición 1:** El entorno de pruebas fue desplegado con éxito por [docker-infra](https://github.com/Danielito2252/docker-infra)[cite: 1].
* **Precondición 2:** Contar con un token de API de pruebas válido.

## 🛤️ Pasos de Ejecución (Steps)
1. Enviar una petición POST a `/api/v1/auth/login` con el payload de prueba.
2. Capturar el código de estado HTTP de la respuesta.
3. Validar la estructura del esquema JSON devuelto.

## 🎯 Resultados Esperados
* El código de estado HTTP devuelto debe ser `200 OK`.
* El campo `authenticated` debe ser igual a `true`.

## 🔗 Enlace al Código de Automatización
* **Ubicación del Script:** [Ver archivo de prueba en cypress-e2e-suite](https://github.com/Danielito2252/cypress-e2e-suite)[cite: 1]