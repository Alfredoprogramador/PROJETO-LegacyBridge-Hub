# LegacyBridge Hub — Arquitetura de Alto Nível

## Problema

Empresas com legados críticos (mainframe, COBOL, VB6, bancos antigos, ERPs legados) precisam integrar e modernizar sem big bang.

## Objetivo arquitetural

- Conectar legado e moderno sem interromper a operação
- Permitir substituição gradual de capacidades legadas
- Governar integrações com observabilidade e segurança

## Camadas

1. **Adapters**
   - Conectores de entrada/saída (REST, gRPC, JDBC/ODBC, SOAP, arquivo)
2. **Canonical Model**
   - Modelo de dados padronizado para reduzir acoplamento com legados
3. **Orquestração**
   - Workflows de longa duração e compensações (Saga)
4. **Inteligência**
   - Sugestão de mapeamento de campos via IA
5. **Modernização**
   - Strangler Fig + Anti-Corruption Layer para migração gradual
6. **Governança**
   - Catálogo, versionamento, políticas e auditoria

## Padrões

- Strangler Fig
- Anti-Corruption Layer
- Saga Pattern
- Change Data Capture (CDC)

## Stack de referência

- Frontend: Next.js + TypeScript + Tailwind + shadcn/ui + React Flow
- Backend: Node.js + NestJS
- Integração: Apache Camel / Spring Integration + REST/gRPC
- Eventos: Kafka + RabbitMQ + Debezium
- Dados: PostgreSQL + MongoDB + Redis
- Orquestração: Temporal
- Observabilidade: OpenTelemetry + Jaeger + Prometheus + Grafana
