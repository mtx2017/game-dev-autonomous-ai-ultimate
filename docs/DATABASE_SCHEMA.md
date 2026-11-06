# Modelo de dados proposto

## Tecnologia
PostgreSQL para serviço multiusuário; SQLite pode servir a protótipo local. A escolha final depende dos requisitos operacionais.

## Entidades
- users: identidade e preferências.
- projects: motor, plataforma, zona, workspace e estado.
- agents: papel, versão, capacidades e limites.
- tasks: objetivo, estado, entradas, saídas e dependências.
- integrations: ferramenta, endpoint referenciado, versão e health.
- approvals: ação, alvo, escopo, solicitante, decisão e validade.
- test_results: suíte, ambiente, resultado e evidências.
- audit_logs: ator, ação, recurso, timestamp e correlation_id.

## Integridade
IDs estáveis, chaves estrangeiras, índices por projeto/estado, timestamps UTC, transações e migrações versionadas.

## Privacidade
Segredos fora das tabelas comuns; armazenar referências a secret manager. Separar dados por projeto e usuário. Definir retenção e exclusão.

## Estado
Modelo lógico, não banco criado.
