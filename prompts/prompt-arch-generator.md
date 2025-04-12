# Nome
Arch Macro View Generator

# Descrição
Geração de um digrama C4 Model representando uma visão macro de arquitetura de um sistema

# Instruções
```
Gerar um diagrama em plantUML (versão 1.2025) representando os componentes macro de uma solução de software. 
Seguir o modelo de formatação e estrutura abaixo

Exemplos

@startuml
!include https://raw.githubusercontent.com/plantuml-stdlib/C4-PlantUML/master/C4_Container.puml

AddElementTag("alterado", \
  $fontColor="black", \
  $bgColor="gold", \
  $legendText="Item alterado", \
)

AddElementTag("novo", \
  $fontColor="black", \
  $bgColor="salmon", \
  $legendText="Item novo", \
)

title Model Context Protocol (MCP)

Person_Ext(user, "Usuário", "Consumidor de serviços GenAI")
Person_Ext(developer, "Desenvolvedor", "Integrador de apps")

System_Boundary(mcp, "Model Context Protocol (MCP)") {
  Container(model_layer, "Model Layer", "AI/ML Models", "Gerencia modelos IA/ML", $tags="novo")
  Container(context_mgmt, "Context Management", "Context Processor", "Gerencia contexto operacional", $tags="novo")
  Container(protocol, "Protocol Interface", "API Gateway", "Define padrões de integração", $tags="novo")
}
Rel(model_layer, context_mgmt, "fornece inferência", "Internal API")
Rel(context_mgmt, protocol, "fornece contexto", "Internal API")
Rel(protocol, model_layer, "envia requisições", "Internal API")

System_Boundary(client, "Client Applications") {
  Container(frontend, "Front-end Application", "React/Angular/Vue", "Interface do usuário", $tags="novo")
}
Rel(frontend, protocol, "consome serviços", "REST API")
Rel(protocol, frontend, "retorna respostas", "REST API")

System_Boundary(storage, "External Storage") {
  Container(postgres, "PostgreSQL", "Relational DB", "Armazena dados estruturados")
  Container(file_server, "File Server", "NFS/S3", "Armazena arquivos binários")
}
Rel(protocol, postgres, "persiste dados", "SQL")
Rel(protocol, file_server, "armazena arquivos", "FTP/HTTP")

System_Boundary(tools, "External Services") {
  Container(jira, "Jira", "Atlassian", "Gerencia tarefas")
  Container(gdrive, "Google Drive", "Google Cloud", "Gerencia documentos")
}
Rel(protocol, jira, "integra tarefas", "REST API")
Rel(protocol, gdrive, "gerencia documentos", "REST API")

Rel(user, frontend, "utiliza", "HTTPS")
Rel(developer, protocol, "integra com", "REST API")

SHOW_LEGEND()
@enduml

```