# System Architecture

```mermaid
flowchart TD

A[Customer] --> B[Chat Interface]

B --> C[Python Backend FastAPI]

C --> D[RAG System]

C --> E[Tools / APIs]

C --> F[Business Rules]

D --> G[LLM API]
E --> G
F --> G

G --> H[Final Response]

H --> A