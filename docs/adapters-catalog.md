# Catálogo Inicial de Adapters

## Objetivo

Padronizar conectores de sistemas legados para exposição controlada em APIs e eventos.

## Adapters previstos (MVP)

| Adapter | Protocolo | Direção | Uso |
|---|---|---|---|
| REST Adapter | HTTP/JSON | In/Out | Integração com APIs modernas |
| gRPC Adapter | gRPC | In/Out | Comunicação performática entre serviços |
| JDBC/ODBC Adapter | SQL | Out | Leitura/escrita em bancos legados |
| File Adapter | CSV/Fixed Width | In/Out | Processamento de arquivos batch |

## Adapters previstos (Fase 2)

| Adapter | Protocolo | Direção | Uso |
|---|---|---|---|
| SOAP Adapter | SOAP/XML | In/Out | Compatibilidade com serviços legados |
| Mainframe Gateway Adapter | CICS/MQ/API | In/Out | Integração com z/OS e AS/400 |

## Convenções mínimas

- Todos os adapters devem mapear para o **Canonical Model**
- Erros devem ser normalizados por código e categoria
- Tracing distribuído deve estar ativo em todos os fluxos
