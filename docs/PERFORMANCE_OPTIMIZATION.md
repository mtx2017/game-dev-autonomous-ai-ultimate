# Otimização de desempenho

## Perfis
LOW, MEDIUM, HIGH e ULTRA são perfis configuráveis; valores concretos devem vir de medições no dispositivo-alvo.

## Técnicas
LOD, frustum/occlusion culling, instancing, batching, streaming, compressão de texturas, pooling, redução de overdraw, simplificação de shaders e controle de partículas.

## Métricas
FPS e frame time, CPU/GPU, RAM/VRAM, draw calls, triângulos, tempo de carregamento, latência e uso de rede.

## Plataformas
Validar separadamente PC, Android/iOS, Roblox e builds Unity. Não extrapolar resultados de um único equipamento.

## Hardware de desenvolvimento
Considerar limites reais de VRAM e memória do equipamento de criação; não presumir que hardware de desenvolvimento representa os dispositivos dos jogadores.

## Gate
Toda otimização deve comparar baseline e resultado, com cena, build, dispositivo e método registrados.
