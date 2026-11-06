# Política GitHub

## Modelo de branches
- `main`: versão estável; protegida.
- `dev`: integração contínua.
- `feature/<tema>`: funcionalidade.
- `fix/<tema>`: correção.
- `qa/<tema>`: validação isolada.

## Fluxo
Issue/requisito → branch → alteração pequena → testes → revisão → PR → aprovação → merge. Para esta skill, o repositório de origem é privado.

## Segurança
- Nunca commitar tokens, chaves, arquivos .env, dumps privados ou dados pessoais.
- Revisar diff antes de push/merge.
- Exigir backup e aprovação para operações destrutivas.
- Não usar force push em main.
- Releases e publicação externa exigem autorização específica.

## Distribuição privada
O titular pode clonar/baixar o pacote para outras contas e computadores próprios, respeitando termos e permissões das plataformas. Repositório privado reduz exposição, mas não impede que alguém com acesso autorizado copie conteúdo.
