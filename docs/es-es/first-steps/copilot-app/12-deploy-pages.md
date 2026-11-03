---
title: "Lección 12 - Publicar el sitio con GitHub Pages"
description: "Usa la aplicación GitHub Copilot para configurar un flujo de trabajo de Pages, revisar su pull request y verificar que Space Quiz está publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publica Space Quiz con GitHub Pages para que tenga un sitio público. Copilot puede preparar el flujo de trabajo y guiarte durante la publicación, pero debes revisar los cambios y confirmar que el sitio está disponible.

En esta lección:

- pedirás a Copilot que configure la publicación con GitHub Pages.
- revisarás el flujo de trabajo y el pull request antes de combinarlo.
- seguirás la publicación y verificarás el sitio publicado.

## Escenario

Space Quiz ya está en un repositorio de GitHub, pero hace falta una forma sencilla de probarlo. Publicar el sitio de un solo archivo con GitHub Pages permite acceder a él desde una URL pública sin añadir un servidor ni una dependencia de ejecución.

## Pide a Copilot que publique el sitio

En la sesión de la aplicación Copilot para `space-quiz`, envía este prompt:

```plaintext
Habilita GitHub Pages para este repositorio. Crea un flujo de trabajo de GitHub Actions que compile el sitio web si es necesario y lo publique en GitHub Pages. Añade un README que describa la aplicación y cómo ejecutarla localmente, si todavía no existe. Crea un pull request con estos cambios y combínalo cuando pasen las comprobaciones obligatorias. Supervisa la publicación hasta que se complete correctamente y, después, indica la URL final del sitio web activo. Si no tienes permiso para habilitar Pages o combinar el pull request, dime exactamente qué debo aprobar o hacer; no indiques que se ha completado correctamente hasta que el sitio esté publicado.
```

![Diagrama en tres etapas: un pull request de space-quiz combinado; una ejecución correcta de GitHub Actions Deploy website con los pasos Build website, Upload artifact y Deploy to Pages; y Space Quiz activo en yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pide al agente que cree y combine un pull request y cambie la configuración de Pages del repositorio. Revisa las diferencias, los permisos de publicación y cualquier solicitud de aprobación de GitHub antes de continuar.

## Revisa el flujo de trabajo y verifica la publicación

1. Confirma que el README solo se ha añadido si el repositorio aún no tenía uno.
2. Revisa los cambios del pull request, incluidos los pasos de compilación y publicación del flujo de trabajo.
3. Combina el pull request únicamente después de que pasen las comprobaciones obligatorias.
4. Sigue la ejecución de publicación de GitHub Actions hasta que se complete correctamente.
5. Abre la URL indicada y confirma que Space Quiz se carga.

Si el agente no puede habilitar Pages o combinar el pull request, sigue las instrucciones concretas que te proporcione. No des la tarea por terminada hasta que la publicación se complete y el sitio activo se cargue.

## Resumen y próximos pasos

Space Quiz ya está disponible como sitio activo y has verificado la publicación, en lugar de confiar únicamente en el informe del agente. Continúa con la [lección 13: Repaso y próximos pasos][next-lesson].

[next-lesson]: ../13-review/
