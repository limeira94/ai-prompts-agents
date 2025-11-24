# AI Prompts and Agents Repository

## Overview

Welcome to the AI Prompts and Agents repository! This repository is a curated collection of prompts and agent configurations designed to assist with a wide range of tasks, from software engineering and cloud architecture to general study and content creation. Our goal is to provide a structured, collaborative space for creating, sharing, and refining high-quality inputs for AI models.

## Prompts vs. Agents

To keep our collection organized, it's important to understand the distinction between `prompts` and `agents`:

-   **Prompts**: These are carefully crafted text inputs designed to elicit a specific type of response from a large language model (LLM). A prompt is typically a single set of instructions, questions, or context that you provide to the AI in a single interaction. They are best for one-off tasks.

-   **Agents**: An agent defines the *persona*, *rules*, and *behavior* of an AI model, turning it into a specialized assistant for a particular role. An agent configuration is more persistent and complex than a prompt. It often includes a system prompt, task-specific instructions, and constraints that guide the AI's responses over a longer conversation or a series of interactions.

In short: a **prompt** is what you *give* to an AI, while an **agent** is what you want the AI to *be*.

## Repository Structure

The repository is organized into three main directories:

```
/
├── README.md
├── prompts/
│   ├── devops/
│   ├── cloud/
│   ├── software-engineering/
│   ├── study/
│   └── general/
├── agents/
│   ├── devops/
│   │   ├── kubernetes-agent.yaml
│   │   └── ci-cd-agent.yaml
│   ├── cloud/
│   │   ├── aws-solutions-architect-agent.yaml
│   ├── education/
│   │   ├── english-teacher-agent.yaml
│   └── code-review/
│       └── senior-reviewer-agent.yaml
└── templates/
    ├── prompt-template.md
    └── agent-template.md
```

-   `/prompts`: Contains standalone prompts, categorized by domain.
-   `/agents`: Contains agent configurations, categorized by role or function.
-   `/templates`: Provides starter templates for creating new prompts and agents.

## How to Contribute

We encourage contributions! Please follow these guidelines to add new content.

### How to Create a New Prompt

1.  **Choose a Category**: Navigate to the most relevant sub-directory inside `/prompts`. If a suitable category doesn't exist, feel free to create one.
2.  **Use the Template**: Copy the contents of `/templates/prompt-template.md` to a new file within your chosen category.
3.  **Name Your File**: Follow the naming conventions described below.
4.  **Write the Prompt**: Fill out the template with your prompt's details, including the title, objective, and the prompt text itself. Be as clear and specific as possible.
5.  **Submit a Pull Request**: Add your new file and submit a pull request for review.

### How to Create a New Agent

1.  **Choose a Category**: Navigate to the most relevant sub-directory inside `/agents`.
2.  **Use the Template**: The `/templates/agent-template.md` provides a basic structure for an agent configuration in YAML format.
3.  **Name Your File**: Create a new `.yaml` file and follow the naming conventions.
4.  **Define the Agent**: Fill out the agent's persona, rules, and capabilities. Define its name, description, and the system-level instructions that will govern its behavior.
5.  **Submit a Pull Request**: Add your new agent configuration and submit a pull request.

## Naming Conventions

To maintain consistency, please adhere to the following naming conventions:

-   **File Names**: Use `kebab-case` (e.g., `kubernetes-deployment-generator.md` or `senior-code-reviewer-agent.yaml`).
-   **Clarity**: Names should clearly and concisely describe the purpose of the prompt or agent.
    -   *Good*: `react-component-generator.md`
    -   *Bad*: `prompt1.md`
-   **Folders**: Categories should also be in `kebab-case`.

## Recommended Tools & Workflow

While not required, the following tools can enhance your experience when working with this repository:

-   **Text Editor**: A good code editor like VS Code with extensions for Markdown and YAML will make editing easier.
-   **AI Playground**: Use an AI playground environment (like the one provided by OpenAI, Google, or Anthropic) to test and refine your prompts and agents before submitting them.
- I recommend using the [Gemini CLI](https://developers.google.com/gemini/cli) to test and iterate on your prompts and agents. This allows you to rapidly test changes in a local environment.
-   **Version Control**: Use Git for version control. Create a new branch for your changes before submitting a pull request.
