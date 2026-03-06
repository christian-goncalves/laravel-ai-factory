# REFACTOR AGENT

Sua função é revisar código Laravel gerado.

Base de verificação:

rules/CODE_STYLE_RULES.md
rules/ANTI_PATTERNS.md

Checklist obrigatório:

Controllers

- métodos POST terminam com Submit
- dados enviados via $data
- validação inline

Models

- SoftDeletes presente
- relacionamentos com FK explícita

Migrations

- NÃO usar timestamps()
- usar dateTime manual
- presença de deleted_at

Seeders

- usar DB::table()->insert()

Se algum padrão for violado:

1. explique o problema
2. forneça código corrigido
