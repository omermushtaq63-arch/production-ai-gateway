# Architecture

Client -> gateway -> validation/rate limiting -> cache -> provider abstraction -> Azure OpenAI or another model provider.

Production hardening can add Microsoft Entra ID/JWT, Key Vault, Redis, Application Insights, Azure Monitor, cost/latency telemetry, and policy-based data boundaries.