# Anthony Chassier

**Développeur C#/.NET et chef de projet technique · Intégration d'IA : LLM local, harnais d'agents, MCP, évaluations**

Je développe en .NET depuis 2007 et j'ai mené des équipes de 2 à 4 développeurs de 2022 à 2025. En 2026, j'intègre l'IA en entreprise. Psychologue de formation, je regarde aussi comment une équipe adopte l'outil : c'est le sujet de CoachIA, plus bas.

`C#` `.NET 10` `ASP.NET Core` `Angular` `SQL Server` · `Claude Code` `MCP` `OpenTelemetry` `Phoenix` `Temporal` `Docker` · `Azure DevOps` `GitHub Actions`

## Deux projets récents

### [SiteGuardian](https://github.com/anthonyC77/SiteGuardian) — des agents qui auditent et corrigent un site, sous contrôle humain

Un premier agent audite un site hébergé sur Kajabi (SEO, liens, accessibilité, sécurité, performance, contenu) et rend un rapport PDF. Un second transforme une demande en langage naturel, « répare le lien YouTube du footer », en plan de correction. Rien n'est écrit sur le site avant qu'un humain ait validé ce plan ; la correction passe ensuite par le serveur MCP officiel de Kajabi.

- **Coûts tenus** : plafonds de jetons et d'appels d'outils par correction, budget en euros par audit.
- **Un modèle par rôle** : Haiku corrige, Sonnet prend le relais au-delà d'un seuil. Un premier tri orthographique se fait en local (Hunspell) avant d'appeler le modèle.
- **Modèle remplaçable** : les agents ne connaissent qu'une interface. Claude aujourd'hui, un modèle local demain, sans toucher aux agents.
- **Écriture verrouillée** : liste blanche des outils d'écriture, revérifiée au moment d'appliquer.
- .NET 10, ASP.NET Core, EF Core + SQLite, SignalR, Angular 19, OAuth 2.1 avec PKCE, QuestPDF · 77 tests xUnit, CI GitHub Actions.

### [CoachIA](https://github.com/anthonyC77/CoachIA) — un harnais qui mesure le travail avec un agent de code

CoachIA lit les sessions Claude Code, l'historique comme le temps réel, les découpe en tâches et mesure ce qui coûte : reprises, échecs d'outils, contexte saturé, mélange Haiku/Sonnet/Opus. Chaque lundi, un bilan cite les vraies tâches de la semaine et réécrit le prompt qui a coûté le plus cher.

- **Observabilité hébergée** : traces OpenTelemetry au format OpenInference, envoyées à Arize Phoenix en Docker local. Par défaut, rien ne quitte le poste.
- **Évaluations** : une campagne mesure l'outil lui-même et rend un code de sortie lisible par une CI (0 rien n'a bougé, 1 un écart à trancher, 2 rien mesuré).
- **MCP écrit à la main** : JSON-RPC 2.0 sur stdio, sans SDK, testé sans lancer de processus.
- **Durable** : le bilan tourne aussi en workflow Temporal, reprenable après panne et planifié le lundi à 8 h.
- .NET 10 ; le noyau ne dépend d'aucun paquet NuGet. Le coach peut parler StarCraft II ou échecs : des « lentilles » changent les mots, jamais les mesures.

## Ma façon de travailler

- Un plan avant le code, une branche par étape, des pull requests relues.
- Des évaluations rejouées à chaque changement. Un feu vert qui ne mesure rien est pire que pas de feu du tout.
- Le modèle choisi selon la tâche et le budget, pas par habitude.

## Avant

- **[Maticulum](https://github.com/Maticulum/Maticulum)** · 2021, formation Alyra · dApp qui délivre des diplômes en NFT sur Polygon, construite à quatre. Solidity, OpenZeppelin, React, web3.
- **[Submarine VR](https://github.com/anthonyC77/Submarine-VR-application)** · 2020, DU Psychologie et réalité virtuelle · application Unity pour Oculus Quest : hang drum jouable, décor sous-marin, shaders.

## Me joindre

[LinkedIn](https://www.linkedin.com/in/anthony-chassier-20a4aa218)
