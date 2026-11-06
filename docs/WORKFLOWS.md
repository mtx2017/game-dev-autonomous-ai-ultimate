# Workflows

Todos os fluxos começam com diagnóstico READ_ONLY e plano. A execução depende do nível de permissão.

## 1. Game Creation
Brief → requisitos → arquitetura → protótipo isolado → implementação → QA → release aprovado.

## 2. Character Creation
Brief visual → referências licenciadas → conceito → modelagem → retopologia/UV → rig → animação → otimização → importação em cópia.

## 3. World Building
Mapa de alto nível → regiões/biomas → blockout → navegação → landmarks → arte → streaming/LOD → testes de performance.

## 4. Monster Creation
Papel de gameplay → silhueta → modelo → rig → estados de IA → ataques → VFX/SFX → testes de leitura e balanceamento.

## 5. Boss Creation
Fases e telegraphs → arena → padrões de ataque → janelas de dano → cooperação/multiplayer → testes de dificuldade e exploits.

## 6. Weapons & Equipment
Requisitos → conceito → modelo → sockets/attachments → atributos → animações → UI → testes de balanceamento.

## 7. Animation
Referência → rig validado → clips → retarget → blending → sincronização de eventos → testes em motor.

## 8. Magic & VFX
Identidade visual → legibilidade → protótipo → partículas/shaders → orçamento de GPU → acessibilidade → teste em dispositivos-alvo.

## 9. Combat Systems
Regras → autoridade servidor/cliente → hit detection → dano → cooldowns → feedback → anti-exploit → regressão.

## 10. Multiplayer
Modelo de autoridade → protocolo → replicação → persistência → reconexão → carga → segurança e latência.

## 11. Testing & QA
Critérios → casos → execução reproduzível → evidências → triagem → correção autorizada → regressão.

## 12. Build & Release
Versões → revisão → testes → artefatos → assinatura/integridade → notas → aprovação → publicação.

## Gate comum
Nenhum fluxo pode pular revisão de licença, segurança, desempenho e critérios de aceite aplicáveis.
