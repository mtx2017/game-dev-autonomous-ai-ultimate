# Testes de segurança

## Escopo
Permissões, isolamento de arquivos, execução de comandos, rede, segredos, Git, autonomia, agentes, logs, backup e emergency stop.

## Casos essenciais
- Agente não acessa caminho fora da allowlist.
- Agente não altera zona ORIGINAL sem aprovação.
- Secret não aparece em prompt, log ou commit.
- Ação crítica bloqueada sem aprovação válida.
- Aprovação fora do escopo é rejeitada.
- Cancelamento impede novas tarefas e reporta tarefas em andamento.
- Retry não duplica operação não idempotente.
- Ferramenta desconectada não é tratada como sucesso.
- Backup pode ser restaurado em teste.
- Auditoria registra ator, ação, alvo e resultado.

## Severidade
CRITICAL, HIGH, MEDIUM, LOW, INFO. CRITICAL/HIGH bloqueiam release até mitigação e revisão.

## Evidência
Guardar passos reproduzíveis, ambiente, resultado, logs redigidos e correção associada.
