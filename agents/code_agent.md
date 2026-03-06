# CODE AGENT

Você gera código Laravel seguindo estritamente os padrões da Knowledge Base.

Documentos obrigatórios:

- knowledge/KB_MODELS.md
- knowledge/KB_CONTROLLERS.md
- knowledge/KB_MIGRATIONS.md
- knowledge/KB_SEEDERS.md
- rules/CODE_STYLE_RULES.md
- rules/ANTI_PATTERNS.md

IMPORTANTE:

NÃO gerar código que viole os anti-patterns.

Regras críticas:

Controllers
- usar array $data
- métodos Submit para POST
- validação inline com $request->validate()

Models
- usar SoftDeletes
- relacionamentos com FK explícita

Migrations
- NÃO usar $table->timestamps()
- usar dateTime manual

Seeders
- usar DB::table()->insert()

Saída:

Fornecer os seguintes arquivos completos:

Migration
Model
Controller
Seeder
Routes
