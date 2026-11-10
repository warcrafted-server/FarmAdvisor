# TODO

## Alta
- Revisar los términos de uso y `robots.txt` de Wowhead Forever y decidir qué se puede rastrear y cómo (tasa, caché, qué datos factuales se pueden redistribuir). Registrar el resultado antes de escribir la herramienta de `tools/`.
- Confirmar en el cliente Forever la versión (1.60.1, Interface 16001) y qué APIs existen: `TooltipDataProcessor.AddTooltipPostCall`, `C_QuestLog`, `C_TradeSkillUI`, `C_Item` y los eventos de botín.
- Proponer estructura de carpetas y plan de la Fase 1 (basados en Lorewake) y esperar el OK.

## Media
- Crear `THIRD_PARTY_NOTICES.md` en cuanto se incorpore material de terceros (revisar antes su licencia).
- Crear `.pkgmeta`, el TOC (`## X-Curse-Project-ID` lo pone el titular) y el workflow del BigWigs packager al publicar una etiqueta (usará los secretos `CF_API_KEY` y `GITHUB_OAUTH`, que configura el titular).
- Rellenar el campo «About» del repositorio en GitHub: `Farm Advisor – Is this mob worth killing? Drops, professions and quests in the tooltip for WoW Forever. / ¿Merece la pena matar a este PNJ? Botín, profesiones y misiones en el tooltip.`
- Capturas de pantalla para los README y CurseForge.

## Descartado
- Licencia PolyForm Noncommercial 1.0.0: sustituida por WNCL-TP-1.0 (la de Lorewake, del sistema central), que cubre uso no comercial y conservación de autoría.
