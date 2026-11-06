# Motor de autonomia

## Níveis
- **0 — READ_ONLY:** leitura e diagnóstico.
- **1 — PLANNING:** planos e propostas, sem escrita.
- **2 — SAFE_EXECUTION:** ações reversíveis em sandbox/cópia autorizada.
- **3 — SUPERVISED_EXECUTION:** execução por etapas com checkpoints.
- **4 — APPROVED_OPERATIONS:** operações críticas previamente aprovadas em escopo específico.

## Ciclo
Perceber → classificar risco → planejar → validar permissões → executar → verificar → registrar → reportar.

## Limites
Tempo, tokens, chamadas, concorrência, tamanho de arquivos, custo monetário e escopo de rede. Limites ausentes devem ser tratados conservadoramente.

## Autocorreção
Permitida apenas em ambiente isolado e dentro do escopo aprovado. Após falhas repetidas, regressão ou mudança de escopo: interromper e solicitar revisão.

## Emergency Stop
Cancelar tarefas, bloquear novas execuções, revogar leases e preservar logs. Confirmar estado final de operações em andamento.

## Estado
Política definida; motor executável não implementado.
