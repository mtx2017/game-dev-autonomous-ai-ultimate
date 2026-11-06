# Arquitetura

## Camadas propostas
1. **Interface:** painel web/desktop, histórico, aprovações e telemetria.
2. **API Gateway:** autenticação, autorização, validação e rate limits.
3. **Orchestrator:** planejamento, filas, dependências, despacho e recuperação.
4. **Agent Runtime:** execução isolada de agentes e contratos.
5. **Tool Adapters:** conectores para motores, DCCs, IA, Git e serviços.
6. **Project Workspace:** cópias de trabalho, artefatos temporários e manifests.
7. **Persistence:** metadados, tarefas, auditoria e referências a arquivos.
8. **Observability:** logs estruturados, métricas, traces e alertas.

## Comunicação
Codex e Claude Code são ambientes independentes. A coordenação exige adaptadores reais, por exemplo API autenticada, MCP compatível, CLI controlada ou serviço de mensagens. Não presumir memória ou comunicação compartilhada nativa.

## Contrato de tarefa
Campos mínimos: task_id, project_id, agent_id, objective, context, inputs, allowed_paths, denied_paths, tools, permission_level, dependencies, acceptance_criteria, timeout, budget_limit.

## Concorrência
- Usar locks por projeto/arquivo quando houver escrita.
- Permitir paralelismo apenas em tarefas independentes.
- Consolidar alterações por branch/patch e revisão.
- Detectar conflito antes de aplicar mudanças.
- Cancelar tarefas dependentes quando uma entrada crítica falhar.

## Resiliência
Retries limitados e idempotentes; backoff; checkpoints; timeouts; circuit breaker; fila de falhas; cancelamento cooperativo. Operações não idempotentes exigem verificação antes de retry.

## Segurança
Autorização por ação e recurso, isolamento de workspace, segredos fora do contexto do agente, logs sem credenciais e trilha de auditoria imutável sempre que viável.

## Status
Arquitetura lógica proposta. Nenhum serviço, banco, runtime ou barramento é criado automaticamente por este documento.
