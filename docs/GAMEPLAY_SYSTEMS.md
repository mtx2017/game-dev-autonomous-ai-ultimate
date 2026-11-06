# Sistemas de gameplay

## Domínios
- Character: movimento, estados, atributos e câmera.
- Class: papéis, progressão e identidade.
- Combat: alvo, hit detection, dano, defesa e autoridade.
- Skill: custo, cooldown, alcance, efeitos e telegraph.
- Enemy AI: percepção, navegação, estados e decisões.
- Boss: fases, padrões, arena e escalonamento.
- Quest: objetivos, diálogo, estado e recompensa.
- Inventory: slots, stack, peso/limites e persistência.
- Equipment: atributos, raridade, sockets e visual.
- Progression: XP, níveis, desbloqueios e curva.
- Economy: fontes, sinks, preços e prevenção de exploits.
- Multiplayer: servidor autoritativo, replicação e reconexão.
- Save: esquema, migração, validação e recuperação.
- Interaction: prompts, alcance, prioridade e acessibilidade.

## Regras por motor
Roblox: Luau, validação no servidor, RemoteEvents/RemoteFunctions com validação e limites. Unity: C#, arquitetura de cenas/componentes e solução de rede escolhida explicitamente.

## Critérios
Testes de estado, abuso/exploit, latência, persistência, acessibilidade e regressão.
