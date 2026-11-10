# Farm Advisor

[English](README.md)

**Farm Advisor** te dice, en el propio tooltip, si merece la pena matar a un PNJ en **World of Warcraft: Forever**. Muestra qué suelta de lo que necesitas para tus misiones y profesiones, con porcentajes de botín que mejoran mientras juegas. Incluye listas de necesidades unificadas, recetas recomendadas para subir más rápido, rutas de farmeo, valor por PNJ con soporte para Auctionator, seguimiento de alts y filtros por ruleset. Se oculta en combate por defecto. Español e inglés.

> **Estado: en planificación (v0.1.0).** Todavía no hay código del addon; este repositorio solo contiene la documentación. La hoja de ruta de abajo es el alcance previsto y puede cambiar.

<!-- Capturas: añade las imágenes en docs/img/ y enlázalas aquí cuando exista el addon. -->
<!-- ![Tooltip](docs/img/tooltip.png) -->
<!-- ![Ventana principal](docs/img/main-window.png) -->
<!-- ![Opciones](docs/img/options.png) -->

## Funciones previstas

**Fase 1 (MVP)**
- Tooltip del PNJ con el botín que te interesa: objetos de misiones activas, materiales de tus profesiones actuales, porcentaje de botín estimado con indicador de confianza y cuántos tienes y te faltan.
- Opcional: mostrar también lo que suelta y podrías aprender más adelante con tus profesiones actuales.
- Se oculta en combate (activado por defecto, configurable).
- Registro de botín propio por PNJ (npcID sacado del GUID): muertes y apariciones por objeto.
- Porcentajes mezclados: tasa a priori de la base de datos combinada con lo observado, `p = (p0*k + obtenidos) / (k + muertes)`, con `k` configurable (por defecto 20). Sin datos propios, solo se muestra el valor de la base de datos.
- Panel de opciones y localización completa en español e inglés (se detecta el idioma del cliente).

**Fase 2** — lista de necesidades unificada (misiones, recetas elegidas, objetivos manuales, campamento), lista inversa de PNJ por objeto necesario (filtrable por zona y nivel), recetas recomendadas para subir de nivel y dónde farmear sus materiales, contador de progreso con aviso opcional al completar.

**Fase 3** — valor por PNJ (oro/hora o puntuación, integración opcional con Auctionator), rutas de farmeo por zona, todos tus personajes (profesiones, recetas, necesidades; «tu alt X lo necesita» en el tooltip), filtros por ruleset (Normal, PvP, Rol, Rol-PvP, Hardcore).

**Fase 4** — ayuda mínima de campamento (qué necesitas para mejorarlo) y lo que falte del aprendizaje futuro.

El addon tendrá una sola ventana principal y un panel de opciones; todo lo no esencial es opcional.

## Requisitos

- Cliente World of Warcraft: Forever (cliente moderno, Interface 16001; por confirmar en el juego).
- Sin dependencias obligatorias. Auctionator es opcional.

## Instalación y uso

Aún no disponible. Se documentarán aquí cuando exista la primera versión jugable.

## Datos

Los datos de botín, recetas y misiones los generará una herramienta aparte en `tools/` y el addon los cargará de forma perezosa. Un dato sin información se muestra como «sin datos», nunca inventado, y cada valor indica su procedencia (base de datos, observado o mezclado). Se están revisando los términos de uso de las fuentes de datos antes de descargar nada.

## Documentación

- [CHANGELOG](CHANGELOG.md) · [TODO](TODO.md)
- Descripción de CurseForge: [EN](docs/CURSEFORGE.en.md) · [ES](docs/CURSEFORGE.es.md)

## Créditos y licencia

**Farm Advisor** está desarrollado y mantenido por **WarCrafted**.
Copyright (C) 2026 WarCrafted.

Licencia [WNCL-TP-1.0](LICENSE): puedes usarlo, estudiarlo, modificarlo y compartirlo gratis con fines no comerciales. Venderlo o cualquier uso comercial requiere permiso por escrito. Solo cubre el material propio; los componentes de terceros conservan su licencia. Es una licencia propia, no una licencia open source aprobada por la OSI.

Las copias y los forks deben conservar esta atribución y enlazar a https://github.com/warcrafted-server/FarmAdvisor.

Datos de juego de World of Warcraft (c) Blizzard Entertainment; proyecto no afiliado.

### Material de terceros

Este proyecto aún no contiene material de terceros. Todo dato o código de terceros se listará aquí y en `THIRD_PARTY_NOTICES.md` antes de añadirlo.
