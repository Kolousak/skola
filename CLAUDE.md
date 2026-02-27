# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a collection of school notes (in Czech) organized by topic. There is no source code, build system, or tests.

## Structure

All infromation about the project you can find in [about](/diplomka/about/) - always read whole folder

- `picovina/` — Markdown notes on biology/ecology topics (bio milk, bio medicine)

## Language

All content is written in Czech (čeština). Responses and new notes should be written in Czech unless instructed otherwise.

## Subagenti (`.claude/agents/`)

Pro akademickou práci jsou k dispozici specializovaní agenti. Claude je automaticky vybírá podle popisu v YAML frontmatter.

### Výzkum a rešerše
| Agent | Model | Kdy použít |
|-------|-------|------------|
| **research-analyst** | sonnet | Komplexní literární rešerše, syntéza poznatků, identifikace trendů |
| **search-specialist** | haiku | Přesné vyhledávání v akademických databázích, boolean dotazy |
| **data-researcher** | haiku | Hledání datasetů, validace datových zdrojů, environmentální databáze |
| **trend-analyst** | haiku | Analýza trendů v environmentálních datech, časové řady, scénáře |

### Data a statistika
| Agent | Model | Kdy použít |
|-------|-------|------------|
| **data-analyst** | haiku | Základní statistika, vizualizace, R kód, korelace, regrese |
| **data-scientist** | sonnet | Pokročilé modely (GLM, GLMM, GAM), cross-validace, ekologické modelování |

### Psaní a syntéza
| Agent | Model | Kdy použít |
|-------|-------|------------|
| **technical-writer** | haiku | Strukturování textu, psaní metodologie, kontrola stylu |
| **knowledge-synthesizer** | sonnet | Syntéza poznatků z více zdrojů, závěry a diskuse |

### Příklady použití
- "Udělej mi rešerši o vlivu urbanizace na holubí populace" → **research-analyst**
- "Najdi datasety o synantropních ptácích v ČR" → **data-researcher**
- "Analyzuj tato data, udělej GLMM" → **data-scientist**
- "Pomoz mi napsat metodologii" → **technical-writer**
- "Shrň poznatky z rešerše do diskuse" → **knowledge-synthesizer**
