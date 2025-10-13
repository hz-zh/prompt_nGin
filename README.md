# LM Prompt Center

A comprehensive prompt management system for categorizing and organizing prompts for Gemini, ChatGPT, and other Large Language Models (LLMs).

## Overview

LM Prompt Center provides a structured approach to managing AI prompts through Markdown files, supporting both system-level prompts and conversational utility prompts for different use cases.

## Structure

- `LLM-prompts/`: Main directory containing all prompt files
  - `system/`: Contains system-level prompts organized by category
    - `coding/`: Programming and development related prompts
    - `documentation+projects/`: Documentation and project management prompts
    - `specialized/`: Specialized domain prompts
    - `writing/`: Writing assistance prompts with style variations
  - `chat-thread/`: Contains utility prompts for specific tasks within conversations
- `archive/`: Contains older or deprecated prompt versions

## Prompt Types

### System Prompts (`LLM-prompts/system/`)

System prompts define the foundational behavior, personality, and capabilities of an LLM. They are typically set once at the beginning of a session and influence all subsequent interactions.

**Categories:**

- **`coding/`**: Programming and development expertise prompts
- **`documentation+projects/`**: Documentation generation and project management prompts  
- **`specialized/`**: Domain-specific expertise prompts (help desk, mathematical notation, etc.)
- **`writing/`**: Writing assistance with different styles and formats
  - **`writing-voice/`**: Specific writing style variations (APA, technical papers, etc.)

**Characteristics:**

- Set the AI's role, personality, or expertise domain
- Define behavioral guidelines and constraints
- Establish context that persists throughout the conversation
- Usually longer and more comprehensive
- Written in Markdown format for human readability

### Chat Thread Utility Prompts (`LLM-prompts/chat-thread/`)

These are shorter, task-specific prompts designed to be used within ongoing conversations to perform specific functions or guide particular interactions.

**Characteristics:**

- Focused on specific tasks or outputs
- Can be inserted mid-conversation
- Often shorter and more directive
- Designed for immediate, specific responses
- Written in Markdown format with clear objectives and requirements

## Usage Guidelines

### System Prompt Implementation

1. Browse system prompts by category in `LLM-prompts/system/`
2. Use for defining AI personality, expertise, and behavioral rules
3. Keep consistent throughout the conversation
4. Copy and paste the entire prompt content as your system message

### Chat Utility Prompt Implementation

1. Use during active conversations for specific tasks
2. Can be chained together for complex workflows
3. Find prompts in `LLM-prompts/chat-thread/` directory
4. Each prompt includes clear objectives and output requirements

## File Format

All prompts are stored in **Markdown format** for:

- **Human readability**: Easy to browse and edit
- **Version control**: Clear diffs when making changes  
- **Flexibility**: Can include formatting, examples, and structured requirements
- **Portability**: Works across different LLM interfaces

## Current Prompts

### System Prompts

- **Coding**: `python_coder_expert.md` - Expert Python development guidance
- **Documentation**: Project summarization, documentation synthesis, and markdown generation
- **Specialized**: Help desk summarization, mathematical notation (LaTeX)
- **Writing**: Report writing, APA style, technical papers, humanization prompts

### Chat Thread Utilities

- **Project Analysis**: `extract_project_json_v2.md` - Comprehensive project documentation extraction

## Getting Started

1. Browse existing prompts in `LLM-prompts/system/` or `LLM-prompts/chat-thread/`
2. Copy the entire content of a relevant prompt file
3. Paste as your system prompt or use during conversation
4. Modify as needed for your specific use case
5. Test prompts with your preferred LLM (ChatGPT, Gemini, Claude, etc.)

## Contributing

When adding new prompts:

1. Choose the appropriate category under `LLM-prompts/system/` or use `chat-thread/`
2. Use Markdown format with clear headings and structure
3. Include usage instructions and expected outcomes
4. Add descriptive filenames that indicate the prompt's purpose
