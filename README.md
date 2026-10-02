# Production AI Gateway

A .NET 8 API gateway pattern for AI workloads with request validation, rate limiting, response caching, provider abstraction, and production observability hooks.

> Portfolio implementation based on professional experience and documented technology areas. No proprietary code or customer data is included.

## Stack
C# / .NET 8 / ASP.NET Core / rate limiting / caching / Azure OpenAI-ready / Docker / observability-ready

## Run
```bash
dotnet restore
dotnet run --project src
```

## API
- GET /health
- POST /api/chat with {"prompt":"Explain RAG in one sentence."}

The local provider makes the gateway runnable without credentials. Production can use Azure OpenAI, Microsoft Entra ID/JWT, Key Vault, Redis, Application Insights, and Azure Monitor.

See docs/architecture.md.
