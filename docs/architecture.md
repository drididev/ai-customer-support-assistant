# System Architecture

```mermaid
flowchart TD

CUS[Customer] --> FRONTEND[Chat Interface]

FRONTEND --> BACKEND[FastAPI Backend]

BACKEND --> AUTH[Authentication]

AUTH --> USERDB[User Database]


BACKEND --> HIST[Conversation]

HIST --> HISTDB[Chat History]

BACKEND --> ORCH[AI Orchestrator]

ORCH --> LLM[LLM]

LLM --> RAG[RAG]

RAG --> VECDB[Vector DB]

LLM --> TOOLS[TOOLS / API]

TOOLS --> ERP[ERP / CRM]

LLM --> GUARD[Guardrails]

GUARD --> VALD[Validation]






