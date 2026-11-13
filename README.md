# Kubernetes AI Agent (CrewAI + Ollama)

An AI agent built with CrewAI that investigates Kubernetes questions and writes a report. It runs on a local LLM through Ollama, so there are no API costs.

## Setup

```bash
pip install crewai
crewai install
```

Create a `.env` file (never commit it) with your Ollama model settings, for example `MODEL=ollama/llama3.2`.

## Run

```bash
crewai run
```

The report is written to the output file defined in `src/devops_ai_project/config/tasks.yaml`.

## Notes

- Uses Python 3.12 (3.15 is too new for some dependencies).
- Small local models can be slow and less reliable for agent tasks.

## Credits

Based on the AI-assisted DevOps series by Abhishek Veeramalla and Krish Naik.
