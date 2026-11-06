# Estrutura de diretórios proposta

```text
game-dev-autonomous-ai-ultimate/
├── SKILL.md
├── AGENTS.md
├── README.md
├── config/
│   ├── manifest.json
│   └── CHANGELOG.md
└── docs/
    ├── ARCHITECTURE.md
    ├── SECURITY.md
    ├── TOOLS.md
    ├── WORKFLOWS.md
    ├── IMPLEMENTATION_PLAN.md
    ├── TESTING.md
    ├── GITHUB.md
    ├── KNOWLEDGE.md
    ├── USER_INTERFACE.md
    ├── API_SPECIFICATION.md
    ├── DATABASE_SCHEMA.md
    ├── AUTONOMY_ENGINE.md
    ├── ASSET_PIPELINE.md
    ├── GAMEPLAY_SYSTEMS.md
    ├── PERFORMANCE_OPTIMIZATION.md
    ├── SECURITY_TESTING.md
    └── RELEASE_AND_DISTRIBUTION.md
```

## Separação
A skill e seus arquivos de configuração ficam separados dos projetos de jogo. Cada projeto terá workspace próprio, com manifest, cópia/branch de desenvolvimento, artefatos, testes e logs. Não armazenar projetos originais dentro do repositório da skill.
