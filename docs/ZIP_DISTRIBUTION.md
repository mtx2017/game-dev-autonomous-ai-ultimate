# ZIP Distribution — GAME DEV AUTONOMOUS AI ULTIMATE

**Status:** specification  
**Version:** 1.0.0  
**Repository oficial:** `mtx2017/game-dev-autonomous-ai-ultimate`  
**Distribution:** ZIP portátil, privado e de uso pessoal

## 1. Objetivo

Definir um pacote ZIP que permita transportar a skill entre computadores e contas próprias, mantendo o GitHub privado como fonte oficial das versões.

O ZIP não deve instalar programas, executar comandos, configurar ferramentas ou modificar projetos automaticamente. A instalação inicial será manual e controlada pelo usuário.

## 2. Estrutura recomendada do pacote

Nome sugerido:

`GAME-DEV-AUTONOMOUS-AI-ULTIMATE-v1.0.0.zip`

Conteúdo interno:

```text
GAME-DEV-AUTONOMOUS-AI-ULTIMATE/
├── README.md
├── SKILL.md
├── AGENTS.md
├── LICENSE
├── CHANGELOG.md
├── manifest.json
├── docs/
│   ├── ARCHITECTURE.md
│   ├── IMPLEMENTATION_PLAN.md
│   ├── SECURITY.md
│   ├── SECURITY_TESTING.md
│   ├── TESTING.md
│   ├── TOOLS.md
│   ├── WORKFLOWS.md
│   └── ...demais documentos oficiais
├── .agents/
│   └── skills/
│       └── game-dev-autonomous-ai-ultimate/
│           └── SKILL.md
└── .claude/
    └── skills/
        └── game-dev-autonomous-ai-ultimate/
            └── SKILL.md
```

As duas cópias de `SKILL.md` devem manter o mesmo conteúdo canônico e os metadados exigidos pelas plataformas. Se uma plataforma exigir ajustes específicos, documentá-los e evitar divergência silenciosa entre as versões.

## 3. Compatibilidade por plataforma

- **Codex:** incluir a skill no caminho de descoberta de projeto `.agents/skills/game-dev-autonomous-ai-ultimate/SKILL.md`.
- **Claude Code:** incluir a skill no caminho de descoberta de projeto `.claude/skills/game-dev-autonomous-ai-ultimate/SKILL.md`.

Esses caminhos tornam o pacote preparado para os mecanismos de descoberta por projeto. A disponibilidade em nível de usuário pode exigir copiar a pasta da skill para o diretório pessoal correspondente de cada ferramenta.

A presença dos arquivos no ZIP não comprova, por si só, que a skill foi instalada ou testada. A compatibilidade deve ser validada separadamente em versões reais do Codex e do Claude Code.

## 4. O que pode entrar no ZIP

Incluir somente componentes necessários para transportar e compreender a skill:

- arquivos de instruções e coordenação;
- documentação técnica e de segurança;
- manifesto e histórico de versão;
- arquivos de compatibilidade do Codex e Claude Code;
- modelos de configuração sem credenciais;
- instruções de instalação manual e validação, quando forem criadas.

## 5. O que não pode entrar no ZIP

Não incluir:

- chaves de API, tokens, senhas, cookies ou credenciais;
- arquivos `.env` reais ou configurações pessoais com segredos;
- pastas `.git`, caches, logs, arquivos temporários e dependências instaladas;
- instaladores de programas ou executáveis não necessários;
- projetos existentes do usuário, incluindo NEXA e Lendas do Infinito: Ascensão;
- arquivos de jogos, mundos, personagens, modelos 3D ou outros ativos privados;
- cópias de ferramentas ou conteúdos de terceiros sem autorização de redistribuição.

## 6. Instalação manual e segura

1. Baixar o ZIP do repositório privado autenticado.
2. Conferir nome, versão e origem do pacote.
3. Extrair em uma pasta temporária para inspeção.
4. Escolher o escopo de instalação: projeto específico ou diretório pessoal da ferramenta.
5. Copiar somente a pasta da skill para o diretório reconhecido pela plataforma.
6. Reiniciar ou atualizar a sessão da ferramenta, se necessário.
7. Confirmar que a skill foi descoberta antes de permitir qualquer execução.
8. Manter o modo de trabalho em leitura/planejamento por padrão.
9. Conceder permissões de escrita, comandos, downloads, publicação ou gastos somente mediante autorização explícita e específica.

Não usar scripts de instalação automática nesta primeira versão.

## 7. Proteção dos projetos

A skill deve permanecer separada dos projetos de jogo. A instalação não deve copiar, mover, renomear, abrir para escrita ou alterar automaticamente qualquer projeto existente.

Antes de uma futura execução com efeitos colaterais, exigir:
- identificação do projeto-alvo;
- confirmação do caminho;
- cópia de segurança ou estratégia de recuperação;
- descrição das alterações planejadas;
- autorização explícita do usuário.

## 8. Versionamento e integridade

- O GitHub privado é a fonte oficial.
- Cada ZIP deve corresponder a uma versão identificada no manifesto e no changelog.
- Não sobrescrever silenciosamente um pacote anterior.
- Registrar data de empacotamento, versão e commit de origem.
- Quando o processo de empacotamento estiver implementado, gerar um checksum SHA-256 e incluí-lo junto ao ZIP.
- Não declarar um ZIP como validado até conferir sua estrutura, arquivos e integridade.

## 9. Processo de publicação do ZIP

1. Revisar os arquivos da versão no repositório.
2. Verificar os metadados e os caminhos de Codex e Claude Code.
3. Fazer uma varredura para detectar segredos e arquivos proibidos.
4. Montar o ZIP com a estrutura definida neste documento.
5. Listar e conferir o conteúdo do arquivo compactado.
6. Gerar e registrar o SHA-256.
7. Testar a extração em uma pasta limpa.
8. Validar a descoberta da skill em cada plataforma, sem abrir projetos reais para escrita.
9. Publicar o ZIP como artefato privado ou release privada, conforme as opções disponíveis no repositório.

## 10. Limites desta especificação

Este documento define o formato e o processo recomendado. Ele **não significa que o ZIP já foi gerado**, que existe um instalador, que a integração entre Codex e Claude Code está ativa ou que a compatibilidade foi testada.

A geração do primeiro ZIP deve ocorrer somente depois da revisão dos arquivos de compatibilidade e da aprovação do usuário para essa etapa.
