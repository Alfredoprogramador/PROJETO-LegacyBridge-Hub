# Projeto LegacyBridge Hub

Plataforma de integração e modernização gradual de sistemas legados.

## Objetivo

O projeto aplica uma abordagem híbrida para conectar sistemas legados a serviços modernos sem interrupção operacional, seguindo modernização progressiva com o padrão **Strangler Fig**.

## Estrutura inicial (monorepo)

```text
legacybridge-hub/
├── apps/
│   ├── frontend/
│   ├── backend/
│   └── integration-engine/
├── packages/
│   ├── shared/
│   ├── adapters/
│   ├── ai-mapping/
│   └── temporal-workflows/
├── infra/
│   ├── terraform/
│   └── kubernetes/
├── docs/
│   ├── architecture.md
│   └── adapters-catalog.md
└── docker-compose.yml
```

## Documentação

- Arquitetura de alto nível: `/docs/architecture.md`
- Catálogo inicial de adapters: `/docs/adapters-catalog.md`

## Ambiente local (compose)

1. Crie o arquivo `.env` copiando `.env.example`
2. Ajuste as credenciais para valores fortes
3. Suba os serviços com `docker compose up -d`
