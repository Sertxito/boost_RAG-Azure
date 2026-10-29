# boost_RAG-Azure

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub Repo](https://img.shields.io/badge/repo-boost__RAG--Azure-blue)](https://github.com/Sertxito/boost_RAG-Azure)

> RAG Builder — Base de Conocimiento Empresarial en ~45 minutos

## Overview

Framework llave en mano para construir sistemas RAG (Retrieval-Augmented Generation) sobre Azure. Conecta documentos empresariales (PDF, Word, Excel, SQL, code) → Azure AI Search con hybrid search → respuestas precisas sobre conocimiento corporativo con citas verificables.

### Key Features

- ✅ **8 Agentes Especializados** — Indexación, búsqueda, síntesis, auditoría
- ✅ **15 Skills Reutilizables** — Modelos reusables para dominios específicos  
- ✅ **Tres Tiers Predefinidos** — Mínima, Estándar, Producción
- ✅ **Hybrid Search** — Búsqueda vector + keyword para máxima precisión
- ✅ **Telemetría Completa** — Observabilidad integrada con Application Insights
- ✅ **Budget Alerts** — Control de costes en tiempo real
- ✅ **Despliegue Automatizado** — Onboarding guiado step-by-step

## Quick Start

### Prerequisites

- Azure subscription
- Azure CLI (`az`) installed
- GitHub CLI (`gh`) authenticated

### Installation

Standalone and self-installable, no MCP required. From the project where you want the RAG agents, skills, prompts and instructions:

```bash
npx github:Sertxito/boost_RAG-Azure --target .   # or: npx boost-rag-azure once published
npx github:Sertxito/boost_RAG-Azure --check      # verify
npx github:Sertxito/boost_RAG-Azure --uninstall  # remove
```

GitHub Copilot / VS Code detects the installed assets automatically (reload the window). They land in `.github/agents`, `.github/skills` (mirrored in `.agents/skills`), `.github/prompts` and `.github/instructions`, prefixed with `rag-` (names that already start with `rag-` are not doubled). Nothing already existing is overwritten: every ignored file is reported with a `[WARN] ... IGNORED` message (use `--force` to overwrite).

To work on the boost itself:

```bash
git clone https://github.com/Sertxito/boost_RAG-Azure.git
cd boost_RAG-Azure
# Follow deployment guide in docs/
```

## Documentation

- [Architecture](docs/ARCHITECTURE.md)
- [Deployment Guide](docs/DEPLOYMENT.md)
- [Configuration](docs/CONFIG.md)

## License

MIT — See [LICENSE](LICENSE)
