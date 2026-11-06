# Especificação de API

## Proposta
REST/JSON para operações e WebSocket/SSE para eventos. OpenAPI deve documentar endpoints e schemas. MCP pode ser usado quando suportado pelo serviço e pelo cliente.

## Recursos conceituais
- `/projects`: metadados e zonas.
- `/agents`: catálogo e capacidades.
- `/tasks`: criação, estado, cancelamento e resultados.
- `/approvals`: solicitações e decisões.
- `/integrations`: status e capabilities.
- `/tests`: execuções e evidências.
- `/audit-logs`: trilha de auditoria.

## Contrato
Toda operação de escrita inclui identidade, projeto, recurso, escopo, permission_level, correlation_id e idempotency_key quando aplicável.

## Segurança
Autenticação forte, RBAC/ABAC, menor privilégio, validação de entrada, rate limiting, proteção contra replay, CORS restrito e logs redigidos.

## Versionamento
Prefixo de versão, compatibilidade documentada, migrações e depreciação planejada.

## Estado
Especificação conceitual; endpoints não existem até implementação e testes.
