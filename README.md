# PM - Kanban with an AI Copilot

A project-management MVP where the interesting part is the AI sidebar: a chat agent that
can create, edit and move Kanban cards on your board through tool calls, not just talk
about them.

## Features

- Kanban board with drag-and-drop cards and renamable columns (Next.js)
- AI chat sidebar: the agent manipulates the board for you - "move everything blocked to
  Done", "create cards for these five tasks" - via structured tool-calling against the API
- Python FastAPI backend serving both the API and the static frontend
- SQLite persistence (multi-user schema, single-user MVP auth)
- Fully Dockerized: one container runs everything

## Stack

Next.js / TypeScript frontend, FastAPI backend, SQLite, OpenRouter-served LLM for the
agent, Docker packaging, uv for Python dependency management.

## Run

Set OPENROUTER_API_KEY in .env at the project root, then build and run the container.
The app serves at / with the API underneath.

---

Built by Nuel Omole - AI automation systems (n8n, LLM pipelines, scraping, outbound).
