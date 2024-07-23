# Local LLM trace stack

## Goal
I want to have a local LLM trace stack that can be used to debug and test LLM applications.
As a proxy to any endpoint so i can just ALWAYS plug and play gpt-3.5 but in reality use whatever, and I want and also log everything.

## Techstack
LiteLLM + Langfuse + whatever they need as one docker compose stack.


## Tips / Debug
- Docker networking: Connect to any container and ping/curl whatever needs to be debugged.

## Ease of use
- Added localhost subdomains to /etc/hosts to make sure all tools can resolve it. Without some tools (like vscode REST client) might not work (reason unknown).
  - ```text
    ::1 litellm.localhost langfuse.localhost
    ```
