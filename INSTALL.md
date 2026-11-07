# INSTALL — GAME DEV AUTONOMOUS AI ULTIMATE

**Versão do guia:** 1.0.0  
**Repositório oficial:** https://github.com/mtx2017/game-dev-autonomous-ai-ultimate  
**Distribuição:** privada, portátil e manual

Este guia orienta a preparação e a instalação manual da skill no Codex ou no Claude Code. A skill não é um instalador de programas e não deve modificar projetos de jogos durante a instalação.

## 1. Antes de começar

- Você precisa estar autenticado no GitHub e ter acesso ao repositório privado.
- O ambiente Codex ou Claude Code precisa conseguir acessar o repositório, diretamente ou por uma cópia local fornecida por você.
- Não compartilhe tokens, senhas, chaves de API ou cookies no chat.
- Não use a pasta de um projeto de jogo como destino da instalação, a menos que escolha conscientemente a instalação por projeto.
- A instalação deve ser feita primeiro em uma pasta temporária de preparação.

## 2. Escolha o escopo

Há dois escopos possíveis:

### Instalação pessoal (recomendada para usar em várias pastas)

- **Codex:** diretório pessoal de skills, normalmente `~/.agents/skills/`.
- **Claude Code:** diretório pessoal de skills, normalmente `~/.claude/skills/`.

A localização exata pode variar conforme o sistema operacional e a configuração da ferramenta. Confirme o diretório existente antes de copiar arquivos.

### Instalação por projeto

- **Codex:** `.agents/skills/game-dev-autonomous-ai-ultimate/` dentro do projeto escolhido.
- **Claude Code:** `.claude/skills/game-dev-autonomous-ai-ultimate/` dentro do projeto escolhido.

A instalação por projeto só deve ocorrer quando você indicar expressamente qual projeto receberá a skill. Não instale dentro de NEXA ou Lendas do Infinito: Ascensão sem autorização específica.

## 3. Prompt pronto para Codex

Copie e cole este texto no Codex:

```text
Quero preparar a instalação da skill GAME DEV AUTONOMOUS AI ULTIMATE a partir do repositório privado:

https://github.com/mtx2017/game-dev-autonomous-ai-ultimate

Siga estas regras:

1. Primeiro verifique se este ambiente consegue acessar o repositório privado usando uma autenticação já configurada. Não peça nem imprima tokens, senhas ou chaves.
2. Se não houver acesso, pare e explique como posso fornecer uma cópia local ou ZIP. Não tente contornar a autenticação.
3. Leia INSTALL.md, README.md, SKILL.md e docs/ZIP_DISTRIBUTION.md.
4. Verifique a estrutura e os metadados da skill. Não presuma compatibilidade só porque os arquivos existem.
5. Identifique o diretório pessoal de skills do Codex neste sistema e confirme o caminho antes de qualquer cópia.
6. Prepare uma cópia de trabalho temporária e mostre a lista de arquivos que seriam instalados.
7. Não instale programas, não execute scripts de instalação, não altere configurações globais e não copie arquivos ainda.
8. Não abra, modifique, mova, renomeie ou sobrescreva projetos existentes. Em especial, preserve integralmente NEXA e Lendas do Infinito: Ascensão.
9. Não inclua credenciais, arquivos .env, caches, dependências, pastas .git ou arquivos privados de projetos.
10. Ao final, apresente o caminho de destino, os arquivos previstos, eventuais incompatibilidades e os passos de instalação.

Pare e aguarde minha autorização explícita antes de copiar qualquer arquivo para o diretório de skills.
```

## 4. Prompt pronto para Claude Code

Copie e cole este texto no Claude Code:

```text
Quero preparar a instalação da skill GAME DEV AUTONOMOUS AI ULTIMATE a partir do repositório privado:

https://github.com/mtx2017/game-dev-autonomous-ai-ultimate

Siga estas regras:

1. Verifique se este ambiente já possui acesso autenticado ao repositório. Nunca solicite, revele ou grave tokens, senhas ou chaves no chat.
2. Se não conseguir acessar o repositório, pare e peça que eu forneça uma cópia local ou ZIP. Não tente contornar permissões.
3. Leia INSTALL.md, README.md, SKILL.md e docs/ZIP_DISTRIBUTION.md.
4. Confira o formato e os metadados exigidos pelo Claude Code. Não declare a instalação compatível ou concluída sem validar.
5. Identifique o diretório pessoal de skills do Claude Code neste sistema e confirme o caminho antes de qualquer cópia.
6. Prepare uma cópia temporária e mostre a lista de arquivos que seriam instalados.
7. Não instale programas, não execute scripts de instalação, não altere configurações globais e não copie arquivos ainda.
8. Não abra, modifique, mova, renomeie ou sobrescreva projetos existentes. Em especial, preserve integralmente NEXA e Lendas do Infinito: Ascensão.
9. Não inclua credenciais, arquivos .env, caches, dependências, pastas .git ou arquivos privados de projetos.
10. Informe o caminho de destino, os arquivos previstos, incompatibilidades e os passos de instalação.

Pare e aguarde minha autorização explícita antes de copiar qualquer arquivo para o diretório de skills.
```

## 5. Validação depois da autorização

Depois que o usuário autorizar a cópia:

1. Copiar somente a pasta da skill para o diretório confirmado.
2. Conferir se o arquivo `SKILL.md` está no caminho correto.
3. Conferir o frontmatter YAML e o conteúdo.
4. Reiniciar ou atualizar a sessão da ferramenta, se necessário.
5. Confirmar que a ferramenta reconhece a skill.
6. Fazer um teste somente de leitura/planejamento, sem modificar projetos.
7. Registrar plataforma, versão da ferramenta, caminho e resultado do teste.

Se qualquer validação falhar, não improvisar mudanças em projetos. Relatar o erro e aguardar instruções.

## 6. Atualização da skill

Para atualizar, compare a versão instalada com a versão do repositório. Preserve configurações locais e não sobrescreva alterações sem mostrar a diferença e obter autorização.

## 7. Limites

Este guia não instala a skill automaticamente, não cria conexão entre Codex e Claude Code e não garante que o ambiente tenha acesso ao repositório privado. O ZIP e os caminhos de instalação precisam ser conferidos antes do uso.

A instalação só estará concluída quando os arquivos forem copiados com autorização e a própria ferramenta reconhecer a skill em um teste controlado.
