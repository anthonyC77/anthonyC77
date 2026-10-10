### Bonjour, je suis Anthony

Développeur C#/.NET depuis 2007, chef de projet technique de 2022 à 2025, psychologue de formation. En 2026, j'intègre l'IA en entreprise. Ci-dessous, mes projets de l'année, menés seul et écrits avec Claude Code : je cadre, je tranche, je relis.

**Projets 2026**

- [**Harnais**](https://github.com/anthonyC77/Harnais) : agents, gardes et évaluations communs à mes dépôts ; le juge des évaluations tourne sur un Qwen local. Dans [mac-ia](https://github.com/anthonyC77/Harnais/tree/main/mac-ia), un pont Anthropic ↔ OpenAI fait piloter Claude Code par Qwen, sur un Mac sans accès Internet : 52 tests sur 52, appels d'outils compris. Temps de réponse réel encore à mesurer.
- [**SiteGuardian**](https://github.com/anthonyC77/SiteGuardian) : audit d'un site Kajabi et corrections en langage naturel, appliquées par MCP seulement après validation humaine. Haiku corrige, Sonnet reprend au-delà de 15 appels d'outils ; le coût estimé d'un audit est plafonné à 0,50 €.
- [**CoachIA**](https://github.com/anthonyC77/CoachIA) : mesure mes sessions Claude Code (reprises, échecs d'outils, contexte saturé), avec des traces OpenTelemetry vers Phoenix en local et un bilan chaque lundi.
- [**Ruche**](https://github.com/anthonyC77/Ruche) : prototype de lecteur 3D (Three.js) qui rejoue un run d'agents, y compris à l'envers, avec les verdicts des évaluations. 14 tests.
- [**Oneiros**](https://github.com/anthonyC77/HermesOneiros) : un agent à mémoire, d'après la documentation d'hermes-agent. Mémoire filtrée et rappel entre sessions sont codés. Pilotage et « rêve » restent à écrire.

**Ma méthode** : un plan avant le code, et des gardes écrites dans le code plutôt que dans le prompt, vérifiées par 28 sondes. Ces sondes ont montré que deux gardes, enregistrées avec des fins de ligne Windows, bloquaient tout depuis le premier commit ; un `.gitattributes` empêche désormais que ça revienne.

<sub>Dans ces dépôts : C# · .NET 10 · Angular · TypeScript · Three.js · Python · Claude Code · MCP · LM Studio · OpenTelemetry · Docker</sub>
