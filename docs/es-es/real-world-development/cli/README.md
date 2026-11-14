---
slug: es-es/real-world-development/cli
title: "GitHub Copilot CLI"
authors:
  - geektrainer
lastUpdated: 2026-06-30
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** incorpora GitHub Copilot a tu terminal como asistente de programación con agentes. Explora bases de código, genera código, ejecuta comandos y se conecta a herramientas externas, todo desde la línea de comandos, para que puedas mantener el flujo sin cambiar a un editor gráfico.

A lo largo de estos ejercicios instalarás y autenticarás Copilot CLI, y después le darás contexto del proyecto con instrucciones personalizadas antes de usar el modo de planificación para generar una funcionalidad de forma deliberada. Conectarás el servidor MCP de Playwright para probar esa funcionalidad en un navegador real y, a continuación, ampliarás Copilot con habilidades de agente reutilizables y agentes personalizados. Por último, explorarás los comandos de barra para gestionar el contexto, los modelos y el uso compartido, y terminarás con un repaso de lo que has creado. También puedes seguir una [serie opcional de tres módulos con GitHub Copilot CLI y Foundry][foundry] para preparar un modelo, crear y desplegar un agente hospedado e integrarlo en el sitio.

## Ejercicios

| Ejercicio | Tema | Descripción |
|----------|-------|-------------|
| [0. Requisitos previos][ex0] | Configuración | Crea tu repositorio y tu codespace |
| [1. Instalar Copilot CLI][ex1] | Instalación | Instala y autentica Copilot CLI |
| [2. Añadir valoraciones con estrellas][ex2] | Funcionalidad | Añade la lógica para calificar elementos con estrellas |
| [3. Modos de agente: Plan y Autopilot][ex3] | Agentes | Usa los modos de planificación y automatización de Copilot |
| [4. Guiar a Copilot con instrucciones personalizadas][ex4] | Contexto | Añade instrucciones para orientar a Copilot durante el desarrollo |
| [5. Personalizar y usar una skill de comprobación de calidad][ex5] | Habilidades | Mejora Copilot con skills especializadas para validación |
| [6. Validar la funcionalidad con Playwright MCP][ex6] | Herramientas externas | Comprueba la experiencia de usuario en un navegador real |
| [7. Crear y usar un agente de QA][ex7] | Pruebas | Crea y utiliza un agente para revisar la calidad del producto |
| [8. Crear y fusionar la PR de la función][ex8] | Flujo de trabajo | Abre, revisa y fusiona la solicitud de cambios de la funcionalidad |
| [9. Comandos de barra en GitHub Copilot CLI][ex9] | Funciones de CLI | Explora contexto, modelos y comandos de barra para potenciar tu flujo |
| [10. Cierre y próximos pasos][ex10] | Resumen | Repasa los puntos clave y decide el siguiente paso |
| [Opcional: incorpora Foundry][foundry] | Agentes hospedados | Prepara un modelo, crea y despliega el agente y conéctalo al sitio web en tres módulos |

## Requisitos previos

Antes de asistir a este taller, asegúrate de tener:

- [ ] Una cuenta de GitHub con un plan activo de **Copilot Student, Pro, Pro+, Business o Enterprise**
- [ ] Conocimientos básicos de operaciones de terminal/línea de comandos
- [ ] Git instalado y configurado

> [!TIP]
> ¿No tienes un plan de pago? Los estudiantes verificados pueden obtener GitHub Copilot gratis a través de [GitHub Education][callout-student-plan-education]. El plan **Copilot Student** incluye las funciones de agente, MCP, revisión de código y Copilot CLI que utiliza este taller, así que puedes completar con él todos los recorridos.

[callout-student-plan-education]: https://github.com/education/students

> [!NOTE]
> Si usas Copilot Business o Copilot Enterprise, asegúrate de que tu administrador haya habilitado Copilot CLI.

## Primeros pasos

**[Empieza con el ejercicio 0: Requisitos previos →][ex0]**

[ex0]: 0-prerequisites/
[ex1]: 1-install-copilot-cli/
[ex2]: 2-add-star-rating/
[ex3]: 3-agent-modes/
[ex4]: 4-custom-instructions/
[ex5]: 5-agent-skills/
[ex6]: 6-mcp-playwright/
[ex7]: 7-qa-agent/
[ex8]: 8-create-pull-request/
[ex9]: 9-cli-power-tools/
[ex10]: 10-review/
[foundry]: 8-foundry-agent/
