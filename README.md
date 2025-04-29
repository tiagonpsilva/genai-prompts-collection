# Coleção de Prompts para GenAI

Uma coleção curada de prompts para Inteligência Artificial Generativa, focada em casos de uso específicos e bem documentados.

## 🎯 Objetivo

Este repositório tem como objetivo fornecer uma coleção organizada de prompts para diferentes casos de uso com IAs generativas. Cada prompt é cuidadosamente documentado e testado para garantir resultados consistentes e úteis.

## 📚 Prompts Disponíveis

### Architecture Haiku Generator
- **Arquivo**: [prompt-architecture-haiku-generator.md](prompts/prompt-architecture-haiku-generator.md)
- **Descrição**: Gera um documento Architecture Haiku a partir de uma descrição de alto nível do projeto, facilitando a comunicação e alinhamento entre stakeholders.

### Modern Data Stack Head Hunter
- **Arquivo**: [prompt_head_modern_data_stack.md](prompts/prompt_head_modern_data_stack.md)
- **Descrição**: Auxilia na avaliação e seleção de profissionais para posições relacionadas à Modern Data Stack.

### API App Generator
- **Arquivo**: [prompt-api-app-generator.md](prompts/prompt-api-app-generator.md)
- **Descrição**: Gera uma aplicação backend RESTful completa com FastAPI, incluindo estrutura de projeto, banco de dados, documentação e testes.

### OpenAPI + Data Schema Generator
- **Arquivo**: [prompt-openapi-data-schema-generator.md](prompts/prompt-openapi-data-schema-generator.md)
- **Descrição**: Gera esquemas de API e modelos de dados a partir de requisitos, incluindo OpenAPI, Postman Collection e MER.

## 📋 Template para Novos Prompts

Para manter a consistência e qualidade dos prompts, utilize o template disponível em [prompt_template.md](prompts/prompt_template.md) ao adicionar novos prompts à coleção.

O template inclui seções para:
- Nome do Prompt
- Descrição
- Instruções detalhadas
  - Contexto
  - Intenção
  - Formato
  - Instruções específicas

## 📚 Estrutura do Repositório

```
genai-prompts/
├── README.md                # Este arquivo
└── prompts/                 # Pasta contendo todos os prompts disponíveis
    ├── prompt-architecture-haiku-generator.md
    ├── prompt_head_modern_data_stack.md
    ├── prompt-api-app-generator.md
    ├── prompt-openapi-data-schema-generator.md
    └── prompt_template.md
```

## 🚀 Como Usar

1. Escolha o prompt adequado da pasta `prompts/` com base no que você deseja gerar
2. Siga as instruções detalhadas no arquivo do prompt
3. Forneça as informações solicitadas no formato especificado
4. Utilize a saída gerada conforme documentado no prompt

## 🤝 Contribuindo

Contribuições são bem-vindas! Para adicionar um novo prompt:

1. Use o template disponível em [prompt_template.md](prompts/prompt_template.md)
2. Crie um novo arquivo na pasta `prompts/`
3. Documente cuidadosamente seu prompt seguindo o formato estabelecido
4. Teste o prompt para garantir resultados consistentes
5. Submeta um Pull Request com suas alterações

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.