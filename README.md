# Crew-Content-Creation Crew

Welcome to the Crew-Content-Creation project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.14 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:
```bash
crewai install
```
### Customizing

- Add your Ollama / model configuration to the `.env` file as needed
- Modify `src/crew_content_creation/config/agents.yaml` to define your agents
- Modify `src/crew_content_creation/config/tasks.yaml` to define your tasks
- Modify `src/crew_content_creation/crew.py` to add your own logic, tools and specific args
- Modify `src/crew_content_creation/main.py` to customize how inputs (like `topic`) are collected

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
$ crewai run
```

This command initializes the Crew-Content-Creation crew, assembling the agents and assigning them tasks as defined in your configuration.

In the current setup:

- You will be prompted for a **topic** at runtime.
- A 3-agent pipeline (researcher → writer → editor) will collaborate.
- The final, polished blog post is written to `output/blog_post.md`.

## Understanding Your Crew

The Crew-Content-Creation crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the ContentCreationCrew Crew or crewAI.
- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.
