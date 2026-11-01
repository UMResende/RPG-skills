# RPG Skills

Repositório pessoal de skills do Claude para RPG de mesa (mestragem, criação de personagens, mundos, sessões).

## Estrutura

```
RPG-skills/
├── README.md
├── skills/
│   ├── _template/        # Modelo para novas skills
│   │   └── SKILL.md
│   └── <nome-da-skill>/
│       ├── SKILL.md      # Obrigatório: frontmatter + instruções
│       ├── references/   # Opcional: regras, tabelas, lore
│       └── scripts/      # Opcional: dados, geradores, utilitários
└── docs/
    └── convencoes.md
```

## Como criar uma skill

1. Copie `skills/_template` para `skills/<nome-em-kebab-case>`.
2. Edite o `SKILL.md` (a `description` é o que dispara a skill: seja específico sobre quando usar).
3. Commit e push.

## Como usar

- **Claude Code:** copie ou faça symlink de `skills/<nome>` para `~/.claude/skills/` (global) ou `.claude/skills/` (projeto).
- **Claude.ai:** compacte a pasta da skill em `.zip` (com a pasta na raiz do zip) e envie em Configurações > Capacidades > Skills.

## Ideias de skills

- `mestre-de-sessao`: preparação de sessão, ganchos, encontros balanceados
- `gerador-de-npc`: NPCs com motivação, segredo e voz
- `criador-de-personagem`: fichas por sistema (D&D 5e, Tormenta20, Ordem Paranormal, etc.)
- `worldbuilding`: facções, locais, linhas do tempo
- `resumo-de-sessao`: transforma notas soltas em crônica e lista de pendências
