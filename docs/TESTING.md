# Estratégia de testes

## Departamentos
1. Funcionalidade e regras de jogo.
2. Integração entre módulos.
3. Multiplayer, replicação e persistência.
4. IA de agentes e ferramentas.
5. Segurança e permissões.
6. Compatibilidade de plataforma/dispositivo.
7. Performance e memória.
8. Assets, rig e animação.
9. Build, instalação e atualização.
10. Recuperação, backup e rollback.

## Tipos
Unitário, integração, sistema, regressão, smoke, carga, compatibilidade, segurança, usabilidade e aceitação.

## Estados
- PASS: evidência reproduzível atende ao critério.
- WARNING: funciona com ressalvas ou cobertura incompleta.
- FAIL: critério não atendido.
- PENDING: ainda não executado ou sem evidência.
- BLOCKED: dependência ou permissão ausente.

## Relatório
Registrar versão, ambiente, dispositivo, passos, resultado esperado/real, logs, screenshots quando aplicável, severidade e vínculo com issue.

Não declarar PASS com base apenas em inspeção visual ou ausência de erro aparente.
