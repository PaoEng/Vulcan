# Vulcan C# Agent

**Modern C# Development with Cloud-Native Architecture (AWS/Azure/Generic)**

Vulcan è un agente esperto di sviluppo C# e .NET 8+ specializzato nella creazione di **codice production-ready** con architetture cloud-native. Supporta AWS, Azure e ambienti provider-agnostic con pattern architetturali puliti, dependency injection, logging strutturato e best practices di sicurezza.

## Caratteristiche Principali

- 🏗️ **Architettura Pulita** — N-Tier, Clean Architecture, Repository Pattern, SOLID principles
- ☁️ **Cloud-Native** — Lambda (AWS), Functions (Azure), serverless e containerizzato (ECS/Container Apps)
- 📊 **Logging & Observability** — Serilog strutturato, correlazione distribuita, telemetria
- 🔒 **Sicurezza** — Credential handling, encryption, vault integration, least privilege
- 💾 **Data Patterns** — Repository Pattern, Entity Framework, DynamoDB, Cosmos DB, LiteDB, MongoDB
- 🔄 **Resilienza** — Retry policies, circuit breakers, timeout handling, graceful degradation

## Casi d'Uso

- **Nuove feature C#** — Da specifica a codice completo production-ready
- **Refactoring architetturale** — Modernizzazione di codice legacy
- **Cloud migration** — Porta codice da on-premise a AWS/Azure
- **Serverless workflows** — Lambda functions, Azure Functions con pattern puliti
- **API REST/gRPC** — Backend completo con autenticazione e validazione
- **Worker/Background jobs** — Processing asincrono, message queues, event-driven
- **Library & NuGet packages** — Codice riutilizzabile con documentazione
- **Infrastructure-as-Code** — CDK (AWS) e Bicep/Terraform (Azure) patterns

## Input

- **Descrizione funzionale** della feature o componente
- **Tipo applicazione**: API, worker, console, library, hybrid
- **Target cloud**: AWS, Azure, o provider-agnostic (Vulcan rileva automaticamente)
- **Storage**: Database, cache, blob storage requirements
- **Integrazioni**: External APIs, message queues, authentication services

## Output

- **Codice C# completo** — Moduli, classi, interfacce pronte per uso
- **Project/assembly structure** — Organizzazione file e namespace
- **Dependency injection setup** — Configuration, registration, lifecycle management
- **Error handling** — Exception patterns, logging, observability
- **Unit test stubs** — Test structure e mock setup
- **Cloud deployment** — CDK/Bicep templates, environment configuration
- **Documentation** — XML comments, architecture diagrams, deployment notes

## Target Cloud

Vulcan rileva automaticamente il target cloud dal contesto:

| Indicatori | Target |
|-----------|--------|
| Lambda, DynamoDB, S3, SQS, SNS, ECS, Fargate, API Gateway | **AWS** |
| Functions, Key Vault, Cosmos DB, Service Bus, Container Apps, Bicep | **Azure** |
| Nessuno specifico, provider-agnostic | **Generic** |

Se non è chiaro, Vulcan chiede una sola domanda: _"AWS, Azure o provider-agnostic?"_

## Stile di Lavoro

- **Veloce**: Consegna codice funzionante rapidamente
- **Fluido**: Transizioni smooth tra componenti
- **Elegante**: Clean code, pattern riconoscibili
- **Pragmatico**: Soluzioni pratiche, non over-engineering

## Installation

Vedi **[Installation Guide](./docs/installation.md)** per le istruzioni passo-passo.

## Quick Start

1. **Descrivi cosa devi costruire**
   ```
   Copilot: /agent
   Seleziona: Vulcan
   
   "Crea un endpoint REST per gestire ordini con validazione,
    logging strutturato e persistenza su Cosmos DB (Azure)"
   ```

2. **Vulcan rileva il target** (Azure da Cosmos DB) e genera codice

3. **Ricevi codice completo** con:
   - OrderController.cs
   - OrderService.cs
   - OrderRepository.cs
   - Dependency injection setup
   - Error handling
   - Unit test stubs

4. **Adatta al tuo progetto** e integra

Per esempi dettagliati, vedi **[Usage Guide](./docs/usage.md)** e **[Examples](./docs/examples.md)**.

## Aree di Specializzazione

- C# 12+ syntax e modern patterns
- .NET 8 features (AOT, performance)
- Async/await, Task-based concurrency
- Entity Framework Core, ADO.NET patterns
- Dependency Injection container setup
- Structured logging (Serilog)
- Configuration management
- Authentication & authorization
- API design & documentation
- Testing strategies (unit, integration)
- Cloud-native deployment

## Integration

**Standalone**: Vulcan genera codice completo e indipendente.

**Collaborativo**: Puoi usare Vulcan per l'implementazione e **Anubis** per code review della sicurezza/quality.

## Support & Resources

- 📖 **[Installation Guide](./docs/installation.md)** — Setup e prerequisites
- 🚀 **[Usage Guide](./docs/usage.md)** — Workflow e comandi
- 💡 **[Examples](./docs/examples.md)** — Scenari real-world
- 🎯 **[Agent Manifest](./Vulcan.agent.md)** — Regole complete e routing

## Next Steps

- Read the **Installation Guide** to get started
- Review the **Usage Guide** for common workflows
- Check **Examples** for real-world scenarios

---

**For information on other agents, see the main [Agents README](../README.md).**
