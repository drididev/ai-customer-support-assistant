# System Architecture

```mermaid
flowchart TD

A[Customer] --> B[Chat Interface Website / Mobile App]

B --> C[Python Backend FastAPI]

C --> D[RAG System]
D --> G[Documents]
G --> H[LLM API]
H --> I[Final Response]

I --> A

C --> E[Tools]
E --> N[Order API]

C --> F[Business Rules]
F --> M[Permissions]



