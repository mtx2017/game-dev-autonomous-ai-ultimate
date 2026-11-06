# Catálogo de agentes

O orquestrador atribui tarefas a especialistas. Um agente não pode ampliar seu próprio escopo nem conceder permissões.

## Contrato comum
Toda tarefa recebe: ID, objetivo, projeto/zona, contexto, entradas, arquivos permitidos/proibidos, ferramentas autorizadas, limites, critérios de aceite e dependências. Toda resposta inclui alterações propostas/realizadas, evidências, testes, riscos e estado.

## Agentes
1. **Game Director / Technical Director** — visão técnica, prioridades, decisões e conflitos.
2. **Game Architect** — arquitetura, módulos, padrões e integração entre sistemas.
3. **Project Planner** — decomposição, dependências, estimativas e marcos.
4. **Research Specialist** — pesquisa de documentação, referências e licenças; registra fontes.
5. **Roblox Luau Engineer** — scripts Luau, serviços, replicação e padrões Roblox.
6. **Unity C# Engineer** — componentes, cenas, ScriptableObjects e arquitetura Unity.
7. **Backend & Multiplayer Engineer** — serviços, persistência, rede, autoridade e sincronização.
8. **Gameplay Engineer** — movimento, interação, progressão e loops de jogo.
9. **Combat Designer** — combate, balanceamento, hitboxes, cooldowns e feedback.
10. **Enemy AI Engineer** — navegação, estados, percepção e comportamento de inimigos.
11. **Quest & Narrative Designer** — missões, diálogos, lore e recompensas.
12. **World Builder** — biomas, regiões, composição, navegação e pontos de interesse.
13. **Character Designer** — silhueta, proporção, conceito e especificações de personagem.
14. **Props & Weapons Artist** — armas, armaduras, objetos e consistência visual.
15. **Blender Technical Artist** — modelagem, topologia, UV, materiais e exportação.
16. **Rigging & Animation Artist** — rigs, retargeting, ciclos e animações.
17. **VFX Artist** — magias, partículas, shaders e legibilidade de efeitos.
18. **UI/UX Designer** — HUD, menus, acessibilidade e fluxos de interface.
19. **Audio Designer** — SFX, música, mixagem e implementação de áudio.
20. **QA Engineer** — testes funcionais, regressão, desempenho e relatórios.
21. **Build & GitHub Engineer** — branches, revisão, CI, builds e releases.

## Regras de delegação
- Um agente responsável por cada entrega; revisores independentes quando o risco justificar.
- Não permitir que agentes concorrentes editem o mesmo arquivo sem coordenação.
- Agentes de pesquisa não executam alterações.
- Agentes de QA não corrigem silenciosamente o objeto que estão validando.
- Agentes de build não publicam nem distribuem sem aprovação específica.
- Se faltar ferramenta, permissão ou contexto, retornar BLOCKED em vez de improvisar.

## Estados de tarefa
QUEUED, READY, RUNNING, BLOCKED, NEEDS_APPROVAL, REVIEW, PASSED, FAILED, CANCELLED.
