# Ferramentas e adaptadores

## Matriz de integração
| Ferramenta | Papel | Integração possível | Verificação obrigatória |
|---|---|---|---|
| Roblox Studio | Motor/editor | Studio API, plugin, MCP ou GUI | versão, instância e place alvo |
| Unity | Motor/editor | Editor scripting, CLI, MCP/GUI | versão, projeto e build target |
| Blender | DCC 3D | Python API, CLI, GUI | versão, arquivo e add-ons |
| Tripo3D | geração 3D | API/web, se disponível | conta, limites, créditos e licença |
| ComfyUI | geração visual | API local/HTTP | endpoint, workflow e VRAM |
| Ollama | modelos locais | API local/CLI | modelo, endpoint e recursos |
| Codex | agente de código | skill/runtime suportado | versão, permissões e workspace |
| Claude Code | agente de código | skills/MCP/CLI suportados | versão, permissões e workspace |
| GitHub | versionamento | API/Git | repo, branch, token e proteção |

## Regras do adaptador
Cada adaptador declara: nome, versão, capabilities, permissões, autenticação, endpoints, limites, formatos, timeout, tratamento de erro e testes de saúde.

## Política
- Verificar a ferramenta real antes de invocar.
- Não inventar endpoints, parâmetros, nomes de ferramentas ou capacidades.
- Preferir API/MCP documentados; GUI é fallback supervisionado.
- Não enviar conteúdo privado a serviços externos sem autorização.
- Registrar custos e limites antes de chamadas pagas.
- Falha de conexão significa BLOCKED, não autorização para instalar outra ferramenta.

## Compatibilidade
A compatibilidade de skills, agentes, MCP e comandos muda entre versões. Validar os formatos nativos de Codex e Claude Code na implementação. Esta especificação não cria integração automaticamente.
