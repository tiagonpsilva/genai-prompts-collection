# GenAI Prompts Collection

## Objetivo

Este repositório contém uma coleção de prompts especializados para modelos de linguagem de grande porte (LLMs), projetados para automatizar a geração de código, documentação e artefatos técnicos. Cada prompt é estruturado para produzir resultados específicos, de acordo com a descrição 

## Instruções de uso

### Pré-requisitos

- Acesso a um modelo de linguagem de grande porte compatível (ChatGPT, Claude, Gemini, etc.)
- Conhecimento básico das tecnologias envolvidas nos projetos gerados

### Como usar os prompts

1. **Selecione o prompt adequado** da pasta `prompts/` com base no que você deseja gerar
2. **Forneça o prompt ao LLM** de sua escolha
3. **Adicione informações específicas** conforme solicitado pelo prompt (requisitos, modelos de dados, etc.)
4. **Receba e utilize os artefatos gerados** pelo modelo

### Prompts disponíveis

#### API App Generator (`prompts/prompt-api-app-generator.md`)
Gera uma aplicação backend RESTful completa baseada nos artefatos fornecidos. O resultado inclui:
- Código-fonte Python/FastAPI com estrutura de projeto completa
- Configuração de banco de dados SQLite com SQLAlchemy
- Documentação (inclusive C4Model)
- Arquivos de configuração (Docker, Terraform, etc.)
- Testes unitários
- Entre outros artefatos

#### OpenAPI + Data Schema Generator (`prompts/prompt-openapi-data-schema-generator.md`)
Gera esquemas de API e modelos de dados a partir de requisitos. Os resultados incluem:
- Arquivo YAML com o schema OpenAPI
- Collection do Postman em JSON
- Modelo Entidade-Relacionamento (MER) em PlantUML
- Schema SQL com dados de exemplo para SQLite

## Estrutura do Repositório
```
genai-prompts/
├── README.md                # Este arquivo
└── prompts/                 # Pasta contendo todos os prompts disponíveis
    ├── prompt-api-app-generator.md
    └── prompt-openapi-data-schema-generator.md
```