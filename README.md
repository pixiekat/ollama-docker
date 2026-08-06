# Katy's Ollama Quickstart

This is just meant to be a small repository to keep my Ollama `docker-compose.yml` file in sync so I can keep the same
environment on both of my machines.

Feel free to take it, use it, fork it, whatever. 🙂

## Setup

Prerequisites:

- Docker
- Docker Compose
- NVIDIA Container Toolkit (`nvidia-container-toolkit` — needed for `runtime: nvidia`).

Getting it running:

- `cp .env.example .env` (open up .env and run `openssl rand[..]` to generate a secret key)
- Make your bind targets with `mkdir -p /path/to/docker_volumes/{ollama_data,openwebui_data}`.
- Run `docker compose up -d`.
- Open OpenWebUI at `http://localhost:3000`.

## Recommended models

These are the models I typically pull down:

- `glm4:9b`
- `qwen3.5:9b`
- `deepseek-coder:6.7b`
- `translategemma:4b`
