---
slug: es-es/real-world-development/cli
title: "GitHub Copilot CLI"
description: "Crea, valida y entrega dos cambios en Tailspin Toys mientras aprendes los modos de Copilot CLI, sus personalizaciones, las herramientas MCP y la automatización de pull requests."
authors:
  - geektrainer
lastUpdated: 2026-09-18
---

**[GitHub Copilot CLI](https://docs.github.com/copilot/concepts/agents/about-copilot-cli)** incorpora GitHub Copilot a tu terminal como asistente de programación con agentes. Explora bases de código, genera código, ejecuta comandos y se conecta a herramientas externas, todo desde la línea de comandos, para que puedas mantener el flujo sin cambiar a un editor gráfico.

El taller sigue un flujo de trabajo continuo en Tailspin Toys. Prepararás el proyecto en GitHub Codespaces, instalarás Copilot CLI y te familiarizarás con él. Después, añadirás valoraciones con estrellas, revisarás el resultado en el navegador y combinarás manualmente tu primer pull request (PR). A continuación, partirás de la incidencia de filtrado, definirás el enfoque en el modo Plan, lo implementarás en el modo Autopilot y lo revisarás en el modo Interactive. Actualizarás las instrucciones del repositorio, personalizarás la skill `quality-checks`, probarás el filtrado con Playwright MCP y crearás un agente de QA. Por último, revisarás el cambio completo y usarás Agent Merge para combinar el PR de filtrado.

Crearás dos PR: uno para las valoraciones con estrellas y otro para el filtrado, que incluirá las actualizaciones de instrucciones y de la skill, el perfil de QA y las pruebas. El trabajo de filtrado y calidad comparte una conversación y una rama para que puedas aprovechar lo aprendido en cada paso. También puedes explorar la [serie opcional de tres módulos con GitHub Copilot CLI y Foundry][foundry].

## Ejercicios

| Ejercicio | Tema | Descripción |
|----------|-------|-------------|
| [0. Requisitos previos][ex0] | Configuración | Crea tu repositorio y Codespace |
| [1. Instalar Copilot CLI][ex1] | Instalación | Instala y autentica Copilot CLI, y familiarízate con la herramienta |
| [2. Añadir valoraciones con estrellas: una mejora rápida][ex2] | Primer cambio | Muestra las valoraciones existentes y el valor alternativo cuando no hay ninguna; después, combina tu primer PR |
| [3. Modos de agente: Plan y Autopilot][ex3] | Modos de agente | Planifica la funcionalidad desde su incidencia, créala con Autopilot y revísala en Interactive |
| [4. Guiar a Copilot con instrucciones personalizadas][ex4] | Contexto | Explora y actualiza las instrucciones y aplícalas al filtrado |
| [5. Personalizar y usar una skill quality-checks][ex5] | Comprobaciones repetibles | Explora la skill existente, cambia el formato del informe y ejecútala |
| [6. Validar la funcionalidad con Playwright MCP][ex6] | Observación en el navegador | Configura MCP en la CLI e inspecciona el comportamiento del filtrado |
| [7. Crear y usar un agente de QA][ex7] | Requisitos y cobertura | Crea y selecciona un perfil especializado y recopila las pruebas de verificación final |
| [8. Crear y combinar el PR de la funcionalidad][ex8] | Revisión y combinación | Revisa todo el cambio, crea el PR y usa Agent Merge |
| [9. Comandos de barra en GitHub Copilot CLI][ex9] | Funciones de la CLI | Explora el contexto, los modelos, el uso compartido y la delegación opcional al agente en la nube |
| [10. Resumen y próximos pasos][ex10] | Resumen | Repasa el flujo de trabajo, las personalizaciones reutilizables y otros recursos |
| [Opcional: incorpora Foundry][foundry] | Agentes hospedados | Prepara un modelo, crea y despliega el concierge y conéctalo al sitio web en tres módulos |

## Requisitos previos

Antes de asistir a este taller, asegúrate de tener:

- [ ] Una cuenta de GitHub con un plan activo de **Copilot Student, Pro, Pro+, Business o Enterprise**
- [ ] Permiso para crear un repositorio y un Codespace
- [ ] Conocimientos básicos de terminal o línea de comandos

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
