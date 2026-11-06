# Segurança e proteção de projetos

## Zonas
- **ORIGINAL:** projeto-fonte; somente leitura por padrão. Escrita exige autorização explícita e específica.
- **DEVELOPMENT:** cópia/branch autorizada para desenvolvimento.
- **SANDBOX:** ambiente descartável para experimentos e testes.

Nunca usar a pasta ORIGINAL como workspace temporário.

## Guardas
- Project Guard: valida projeto e caminhos permitidos.
- Sandbox Guard: confirma isolamento e diretório de trabalho.
- Permission Guard: valida modo e autorização.
- API Guard: protege tokens, escopos e limites.
- Git Guard: bloqueia operações de risco sem aprovação.
- Backup Guard: exige backup verificável antes de mudanças relevantes.
- Agent Monitor: registra ações, ferramentas e consumo.
- Emergency Stop: cancela tarefas e bloqueia novas operações.

## Aprovação específica
Exigir autorização clara antes de: instalar/baixar; executar comandos com efeitos externos; alterar ORIGINAL; apagar/mover/sobrescrever; publicar; criar releases; alterar permissões; enviar dados a terceiros; consumir créditos pagos; compras; deploy; migrações destrutivas.

A aprovação deve identificar ação, alvo, escopo e, quando relevante, duração/limite. Uma aprovação não autoriza ações futuras diferentes.

## Credenciais
Usar armazenamento seguro do ambiente. Nunca incluir secrets em código, prompts compartilhados, issues públicas, logs ou commits. Aplicar menor privilégio, rotação e revogação.

## Git e backups
Usar branches de trabalho, commits pequenos, revisão e proteção de main. Antes de mudanças relevantes, confirmar backup e procedimento de restauração. Não usar force push sem aprovação explícita.

## Incidente
Parar execução, preservar logs, não tentar ocultar ou corrigir evidências, informar o usuário e propor contenção/rollback. Não retomar até autorização.

## Limite
Estas regras são especificação. A proteção efetiva depende de controles implementados no runtime e nas ferramentas conectadas.
