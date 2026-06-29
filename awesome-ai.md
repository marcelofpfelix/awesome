# Awesome AI

A curated list of open-source-first AI agent, coding, memory, retrieval,
workflow, voice, and evaluation tools.

Source entries link directly to their upstream repository and state the type of
app. Explicit non-source exceptions are isolated in their own section. Token,
memory, RAG, or runtime behavior is called out where relevant.

## Contents

- [Coding Agents And Agent Frameworks](#coding-agents-and-agent-frameworks)
- [Agent Session Managers And Parallel UIs](#agent-session-managers-and-parallel-uis)
- [Agent Runtimes And Assistant Platforms](#agent-runtimes-and-assistant-platforms)
- [Memory And Knowledge Stores](#memory-and-knowledge-stores)
- [RAG And Documentation Retrieval](#rag-and-documentation-retrieval)
- [Vector Stores And Retrieval Infrastructure](#vector-stores-and-retrieval-infrastructure)
- [Token-Saving Search And Code Intelligence](#token-saving-search-and-code-intelligence)
- [Structured Outputs](#structured-outputs)
- [MCP, Connectors, And Protocols](#mcp-connectors-and-protocols)
- [Task Management](#task-management)
- [Workflow Orchestration](#workflow-orchestration)
- [Skills And Agent Packs](#skills-and-agent-packs)
- [Browser Automation And Proof](#browser-automation-and-proof)
- [Web Automation And CLI Generation](#web-automation-and-cli-generation)
- [Voice, Multimodal, And Realtime Agents](#voice-multimodal-and-realtime-agents)
- [Local Model Runtimes And App Platforms](#local-model-runtimes-and-app-platforms)
- [Sandboxes, Guardrails, And Policy](#sandboxes-guardrails-and-policy)
- [Evaluation, Observability, And Model Routing](#evaluation-observability-and-model-routing)
- [Non-Source Utilities](#non-source-utilities)
- [Reference Lists And Research](#reference-lists-and-research)

## Coding Agents And Agent Frameworks

- [OpenCode](https://github.com/sst/opencode) [![stars](https://img.shields.io/github/stars/sst/opencode?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/sst/opencode) [![commits](https://img.shields.io/github/commit-activity/m/sst/opencode?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/sst/opencode): Type: terminal coding-agent
  `cli` `daemon` `mcp` `plugin` `skill`.
  CLI/TUI and server. Runs agent sessions over local repositories with skills,
  MCP, plugins, JSON output, and warm-server mode. Token note: can reduce repeat
  startup and MCP context cost by using `opencode serve` plus attached runs.
- [Codex](https://github.com/openai/codex) [![stars](https://img.shields.io/github/stars/openai/codex?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openai/codex) [![commits](https://img.shields.io/github/commit-activity/m/openai/codex?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openai/codex): Type:
  `cli` `mcp` `plugin` `skill` `daemon`.
  terminal coding-agent. Runs repository-aware coding sessions with tool use,
  local edits, approvals, validation commands, skills, plugins, and MCP
  connectors.
- [Claude Code](https://github.com/anthropics/claude-code) [![stars](https://img.shields.io/github/stars/anthropics/claude-code?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/anthropics/claude-code) [![commits](https://img.shields.io/github/commit-activity/m/anthropics/claude-code?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/anthropics/claude-code): Type:
  `cli` `plugin` `daemon`.
  terminal coding-agent. Runs agentic coding workflows over local repositories,
  shell commands, git operations, and editor-style code changes. License note:
  review source and licensing terms before treating it like an ordinary
  open-source dependency.
- [Oh My Pi](https://github.com/can1357/oh-my-pi) [![stars](https://img.shields.io/github/stars/can1357/oh-my-pi?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/can1357/oh-my-pi) [![commits](https://img.shields.io/github/commit-activity/m/can1357/oh-my-pi?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/can1357/oh-my-pi): Type:
  `cli` `plugin` `daemon` `sdk`.
  terminal coding-agent. Provides hash-anchored edits, an optimized tool
  harness, LSP, Python, browser tooling, subagents, and related agent
  workflow features.
- [Pi Agent Harness](https://github.com/earendil-works/pi) [![stars](https://img.shields.io/github/stars/earendil-works/pi?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/earendil-works/pi) [![commits](https://img.shields.io/github/commit-activity/m/earendil-works/pi?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/earendil-works/pi): Type:
  `cli` `daemon` `mcp` `plugin` `sdk`.
  coding-agent CLI, TUI, and runtime. Provides repository-aware agent execution,
  a unified multi-provider LLM API, configurable tool execution, JSON stream
  output, subagents, MCP integration, shell/code/browser tools, and agent loop
  primitives. Safety note: the project states that Pi runs with the launching
  user's permissions unless sandboxed externally, so review permission
  boundaries before broad use.
- [Gemini CLI](https://github.com/google-gemini/gemini-cli) [![stars](https://img.shields.io/github/stars/google-gemini/gemini-cli?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/google-gemini/gemini-cli) [![commits](https://img.shields.io/github/commit-activity/m/google-gemini/gemini-cli?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/google-gemini/gemini-cli): Type:
  `cli` `daemon`.
  terminal coding-agent. Brings Gemini-backed repository assistance, tool use,
  and automation directly into the shell.
- [Qwen Code](https://github.com/QwenLM/qwen-code) [![stars](https://img.shields.io/github/stars/QwenLM/qwen-code?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/QwenLM/qwen-code) [![commits](https://img.shields.io/github/commit-activity/m/QwenLM/qwen-code?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/QwenLM/qwen-code): Type:
  `cli` `daemon`.
  terminal coding-agent. Open-source coding assistant for Qwen models and
  compatible local or hosted development workflows.
- [Goose](https://github.com/block/goose) [![stars](https://img.shields.io/github/stars/block/goose?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/block/goose) [![commits](https://img.shields.io/github/commit-activity/m/block/goose?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/block/goose): Type: local AI agent CLI and desktop
  `cli`.
  app. Runs headless or interactive engineering tasks with tool use and
  extension support.
- [Aider](https://github.com/Aider-AI/aider) [![stars](https://img.shields.io/github/stars/Aider-AI/aider?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Aider-AI/aider) [![commits](https://img.shields.io/github/commit-activity/m/Aider-AI/aider?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Aider-AI/aider): Type: terminal pair-programming
  `cli` `plugin`.
  CLI. Edits known files and can loop on lint/test commands. Token note: works
  best when the file set and validation signal are narrow.
- [OpenHands](https://github.com/All-Hands-AI/OpenHands) [![stars](https://img.shields.io/github/stars/All-Hands-AI/OpenHands?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/All-Hands-AI/OpenHands) [![commits](https://img.shields.io/github/commit-activity/m/All-Hands-AI/OpenHands?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/All-Hands-AI/OpenHands): Type: autonomous
  `cli`.
  software-engineering agent platform. Runs coding tasks in a controlled
  workspace with CLI/headless modes.
- [SWE-agent](https://github.com/SWE-agent/SWE-agent) [![stars](https://img.shields.io/github/stars/SWE-agent/SWE-agent?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/SWE-agent/SWE-agent) [![commits](https://img.shields.io/github/commit-activity/m/SWE-agent/SWE-agent?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/SWE-agent/SWE-agent): Type: software
  `daemon`.
  engineering benchmark and repair agent. Runs batch/headless issue-resolution
  workflows, commonly with SWE-bench style tasks.
- [Cline](https://github.com/cline/cline) [![stars](https://img.shields.io/github/stars/cline/cline?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/cline/cline) [![commits](https://img.shields.io/github/commit-activity/m/cline/cline?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/cline/cline): Type:
  `cli` `plugin` `sdk`.
  autonomous coding agent, SDK, IDE extension, and CLI assistant. Provides
  editor-integrated planning, tool use, command execution, and code changes.
- [Roo Code](https://github.com/RooCodeInc/Roo-Code) [![stars](https://img.shields.io/github/stars/RooCodeInc/Roo-Code?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/RooCodeInc/Roo-Code) [![commits](https://img.shields.io/github/commit-activity/m/RooCodeInc/Roo-Code?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/RooCodeInc/Roo-Code): Type:
  `plugin` `daemon`.
  Cline-derived editor-agent workflow. Provides multi-mode coding assistance
  and role-oriented agent flows. Status note: repository is archived as of the
  2026-06-27 GitHub check.
- [Continue](https://github.com/continuedev/continue) [![stars](https://img.shields.io/github/stars/continuedev/continue?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/continuedev/continue) [![commits](https://img.shields.io/github/commit-activity/m/continuedev/continue?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/continuedev/continue): Type:
  `plugin` `daemon` `sdk`.
  open-source IDE assistant and coding-agent platform. Provides editor-native
  chat, autocomplete, custom model routing, and agent workflows.
- [smolagents](https://github.com/huggingface/smolagents) [![stars](https://img.shields.io/github/stars/huggingface/smolagents?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/huggingface/smolagents) [![commits](https://img.shields.io/github/commit-activity/m/huggingface/smolagents?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/huggingface/smolagents): Type: Python agent
  `sdk`.
  framework/library. Builds code and tool-calling agents with a small framework
  surface.
- [PydanticAI](https://github.com/pydantic/pydantic-ai) [![stars](https://img.shields.io/github/stars/pydantic/pydantic-ai?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/pydantic/pydantic-ai) [![commits](https://img.shields.io/github/commit-activity/m/pydantic/pydantic-ai?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/pydantic/pydantic-ai): Type:
  `sdk`.
  typed Python agent framework. Builds agentic applications with Pydantic-style
  schemas, dependency injection, tool calls, and testable contracts.
- [Monty](https://github.com/pydantic/monty) [![stars](https://img.shields.io/github/stars/pydantic/monty?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/pydantic/monty) [![commits](https://img.shields.io/github/commit-activity/m/pydantic/monty?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/pydantic/monty): Type:
  `sdk` `daemon`.
  experimental secure Python interpreter in Rust for agent-written code. Useful
  when an agent needs fast, controlled Python execution without a full container
  sandbox; not a replacement for PydanticAI or general workflow orchestration.
- [AutoGen](https://github.com/microsoft/autogen) [![stars](https://img.shields.io/github/stars/microsoft/autogen?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/microsoft/autogen) [![commits](https://img.shields.io/github/commit-activity/m/microsoft/autogen?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/microsoft/autogen): Type:
  `plugin` `sdk` `daemon`.
  multi-agent programming framework. Provides conversational agents, tool use,
  orchestration patterns, and reference designs for agentic AI systems.
- [Semantic Kernel](https://github.com/microsoft/semantic-kernel) [![stars](https://img.shields.io/github/stars/microsoft/semantic-kernel?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/microsoft/semantic-kernel) [![commits](https://img.shields.io/github/commit-activity/m/microsoft/semantic-kernel?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/microsoft/semantic-kernel): Type:
  `plugin` `sdk` `daemon` `lib`.
  enterprise agent and AI app SDK. Provides agents, planners, connectors,
  memory patterns, and .NET/Python/Java application integration. Stack note:
  important for enterprise and .NET-heavy systems, but overlaps with
  PydanticAI, LangGraph, AutoGen, CrewAI, and other app frameworks.
- [CrewAI](https://github.com/crewAIInc/crewAI) [![stars](https://img.shields.io/github/stars/crewAIInc/crewAI?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/crewAIInc/crewAI) [![commits](https://img.shields.io/github/commit-activity/m/crewAIInc/crewAI?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/crewAIInc/crewAI): Type:
  `sdk` `daemon`.
  role-agent orchestration framework. Coordinates multiple agents with
  delegated tasks, crews, flows, tools, and process-level control.
- [Mastra](https://github.com/mastra-ai/mastra) [![stars](https://img.shields.io/github/stars/mastra-ai/mastra?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mastra-ai/mastra) [![commits](https://img.shields.io/github/commit-activity/m/mastra-ai/mastra?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mastra-ai/mastra): Type:
  `sdk` `daemon` `lib`.
  TypeScript AI application and agent framework. Builds agents, workflows,
  RAG, tool calls, evaluations, and deployment-oriented AI app backends.
- [VoltAgent](https://github.com/VoltAgent/voltagent) [![stars](https://img.shields.io/github/stars/VoltAgent/voltagent?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/VoltAgent/voltagent) [![commits](https://img.shields.io/github/commit-activity/m/VoltAgent/voltagent?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/VoltAgent/voltagent): Type:
  `plugin` `sdk`.
  TypeScript agent engineering platform. Provides agent framework primitives,
  tooling, observability patterns, and app-oriented agent development.
- [LangChain](https://github.com/langchain-ai/langchain) [![stars](https://img.shields.io/github/stars/langchain-ai/langchain?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langchain-ai/langchain) [![commits](https://img.shields.io/github/commit-activity/m/langchain-ai/langchain?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langchain-ai/langchain): Type:
  `plugin` `sdk` `daemon` `lib`.
  LLM application and agent framework. Provides model, tool, retriever, vector
  store, and integration abstractions for building LLM-powered apps. RAG note:
  useful plumbing for selective retrieval, but not a memory store by itself.
- [LangGraph](https://github.com/langchain-ai/langgraph) [![stars](https://img.shields.io/github/stars/langchain-ai/langgraph?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langchain-ai/langgraph) [![commits](https://img.shields.io/github/commit-activity/m/langchain-ai/langgraph?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langchain-ai/langgraph): Type:
  `sdk` `daemon`.
  stateful agent workflow framework. Builds graph-shaped, controllable agent
  loops with persistence/checkpointing patterns. Memory type: structured
  state/checkpoint memory. Token note: supports message trimming and durable
  state so long runs do not depend only on chat history.
- [DeepAgents](https://github.com/langchain-ai/deepagents) [![stars](https://img.shields.io/github/stars/langchain-ai/deepagents?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langchain-ai/deepagents) [![commits](https://img.shields.io/github/commit-activity/m/langchain-ai/deepagents?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langchain-ai/deepagents): Type:
  `skill` `daemon`.
  batteries-included agent harness. Adds planning, subagents, filesystem
  access, context management, persistent memory, human-in-the-loop controls,
  tools, and skills on top of LangChain/LangGraph. Token note: summarizes long
  threads and can offload tool outputs to disk.
- [hermes-agent](https://github.com/NousResearch/hermes-agent) [![stars](https://img.shields.io/github/stars/NousResearch/hermes-agent?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/NousResearch/hermes-agent) [![commits](https://img.shields.io/github/commit-activity/m/NousResearch/hermes-agent?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/NousResearch/hermes-agent): Type: agent
  `sdk` `daemon` `lib`.
  framework/reference implementation. Tracked separately from the local
  Codex/Hermes workflow layer.

[Back to top](#awesome-ai)

## Agent Session Managers And Parallel UIs

- [cmux](https://github.com/manaflow-ai/cmux) [![stars](https://img.shields.io/github/stars/manaflow-ai/cmux?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/manaflow-ai/cmux) [![commits](https://img.shields.io/github/commit-activity/m/manaflow-ai/cmux?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/manaflow-ai/cmux): Type: multi-agent coding UI and
  `cli` `daemon` `plugin`.
  terminal workflow tool. Helps run, compare, and manage coding-agent sessions
  side by side. Runtime note: useful for parallel exploration or review, but it
  raises review and merge cost if agents edit overlapping files.
- [tmux Claude session manager](https://github.com/craftzdog/tmux-claude-session-manager) [![stars](https://img.shields.io/github/stars/craftzdog/tmux-claude-session-manager?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/craftzdog/tmux-claude-session-manager) [![commits](https://img.shields.io/github/commit-activity/m/craftzdog/tmux-claude-session-manager?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/craftzdog/tmux-claude-session-manager):
  `cli` `plugin`.
  Type: tmux session manager for Claude Code. Runs many Claude Code sessions
  across projects, tracks done vs running sessions, and jumps into a selected
  session from a popup.
- [OpenSessions](https://github.com/Ataraxy-Labs/opensessions) [![stars](https://img.shields.io/github/stars/Ataraxy-Labs/opensessions?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Ataraxy-Labs/opensessions) [![commits](https://img.shields.io/github/commit-activity/m/Ataraxy-Labs/opensessions?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Ataraxy-Labs/opensessions): Type: tmux
  `cli` `plugin`.
  sidebar for coding agents. Tracks Amp, Claude Code, Codex, and OpenCode
  sessions with per-thread markers, a local HTTP API, and live session state.
  License note: GitHub does not report a license, but the source is public.
- [Crabwalk](https://github.com/crabwise-ai/crabwalk) [![stars](https://img.shields.io/github/stars/crabwise-ai/crabwalk?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/crabwise-ai/crabwalk) [![commits](https://img.shields.io/github/commit-activity/m/crabwise-ai/crabwalk?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/crabwise-ai/crabwalk): Type: realtime companion
  `plugin` `cli` `sdk`.
  monitor for OpenClaw agents. Helps watch agent activity while work is running
  outside the main chat.
- [Herdr](https://github.com/ogulcancelik/herdr) [![stars](https://img.shields.io/github/stars/ogulcancelik/herdr?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ogulcancelik/herdr) [![commits](https://img.shields.io/github/commit-activity/m/ogulcancelik/herdr?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ogulcancelik/herdr): Type: terminal agent
  `cli` `plugin`.
  multiplexer. Runs and coordinates multiple agent sessions from the terminal.
  License note: GitHub classifies the license as `Other`; review before
  production use.

[Back to top](#awesome-ai)

## Agent Runtimes And Assistant Platforms

- [OpenClaw](https://github.com/openclaw/openclaw) [![stars](https://img.shields.io/github/stars/openclaw/openclaw?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openclaw/openclaw) [![commits](https://img.shields.io/github/commit-activity/m/openclaw/openclaw?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openclaw/openclaw): Type: local-first personal
  `daemon` `skill` `plugin` `sdk`.
  assistant runtime and daemon. Provides gateway, channels, tools, skills,
  sessions, apps/nodes, cron, webhooks, and mobile/desktop surfaces. Memory
  note: has local runtime state and can integrate external memory, but remote
  channel retention should be audited before saving tool/system transcripts.
- [Paperclip](https://github.com/paperclipai/paperclip) [![stars](https://img.shields.io/github/stars/paperclipai/paperclip?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/paperclipai/paperclip) [![commits](https://img.shields.io/github/commit-activity/m/paperclipai/paperclip?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/paperclipai/paperclip): Type:
  `daemon` `plugin`.
  open-source app for managing workplace agents. Provides an agent management
  surface for teams and workspaces; use as an agent-ops platform, not as a
  replacement for the primary coding CLI.
- [Gitagent](https://github.com/open-gitagent/gitagent) [![stars](https://img.shields.io/github/stars/open-gitagent/gitagent?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/open-gitagent/gitagent) [![commits](https://img.shields.io/github/commit-activity/m/open-gitagent/gitagent?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/open-gitagent/gitagent): Type: git-native agent
  `skill` `plugin` `sdk` `daemon`.
  packaging framework. Stores identity, rules, memory, skills, tools, hooks,
  workflows, agents, and compliance metadata in a repo. Memory note: treats the
  repository as the durable agent state source.
- [OpenAI Symphony](https://github.com/openai/symphony) [![stars](https://img.shields.io/github/stars/openai/symphony?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openai/symphony) [![commits](https://img.shields.io/github/commit-activity/m/openai/symphony?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openai/symphony): Type: autonomous
  `daemon`.
  engineering workflow platform. Runs isolated implementation tasks with
  Linear-backed work and CI/PR proof.
- [Cloudflare Agents](https://github.com/cloudflare/agents) [![stars](https://img.shields.io/github/stars/cloudflare/agents?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/cloudflare/agents) [![commits](https://img.shields.io/github/commit-activity/m/cloudflare/agents?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/cloudflare/agents): Type:
  `daemon` `sdk`.
  deployable agent runtime for Cloudflare Workers. Uses Durable Objects,
  Workers, and the Cloudflare platform for stateful agents, realtime
  interactions, and production deployment patterns.

[Back to top](#awesome-ai)

## Memory And Knowledge Stores

- [Codebase-Memory MCP](https://github.com/DeusData/codebase-memory-mcp) [![stars](https://img.shields.io/github/stars/DeusData/codebase-memory-mcp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/DeusData/codebase-memory-mcp) [![commits](https://img.shields.io/github/commit-activity/m/DeusData/codebase-memory-mcp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/DeusData/codebase-memory-mcp): Type:
  `cli` `mcp` `daemon`.
  persistent codebase memory MCP and CLI. Indexes repositories into a local
  graph store for architecture discovery, impact analysis, and cross-repo maps.
  Memory type: graph/codebase memory, not personal chat memory. Token note:
  saves tokens when it replaces repeated full-repo reading; stale indexes and
  graph misses still require source verification.
- [CodeGraph](https://github.com/colbymchenry/codegraph) [![stars](https://img.shields.io/github/stars/colbymchenry/codegraph?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/colbymchenry/codegraph) [![commits](https://img.shields.io/github/commit-activity/m/colbymchenry/codegraph?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/colbymchenry/codegraph): Type: local code
  `plugin` `daemon`.
  knowledge-graph index for coding agents. Auto-syncs on code changes for
  Claude Code, Codex, Gemini, Cursor, OpenCode, Kiro, and similar tools. Memory
  type: local code graph. Token note: reduces repeated tool calls and broad
  source reads when graph queries answer impact questions.
- [Cognee](https://github.com/topoteretes/cognee) [![stars](https://img.shields.io/github/stars/topoteretes/cognee?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/topoteretes/cognee) [![commits](https://img.shields.io/github/commit-activity/m/topoteretes/cognee?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/topoteretes/cognee): Type: AI memory platform for
  `plugin` `daemon`.
  agents. Provides persistent long-term memory across sessions with a
  self-hosted knowledge-graph engine. Memory type: long-term graph memory.
- [MemPalace](https://github.com/MemPalace/mempalace) [![stars](https://img.shields.io/github/stars/MemPalace/mempalace?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/MemPalace/mempalace) [![commits](https://img.shields.io/github/commit-activity/m/MemPalace/mempalace?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/MemPalace/mempalace): Type: open-source AI
  `plugin` `daemon`.
  memory system. Provides a memory layer for agents and applications. Memory
  type: agent memory store.
- [mem0](https://github.com/mem0ai/mem0) [![stars](https://img.shields.io/github/stars/mem0ai/mem0?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mem0ai/mem0) [![commits](https://img.shields.io/github/commit-activity/m/mem0ai/mem0?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mem0ai/mem0): Type:
  `daemon` `sdk` `lib`.
  universal memory layer for AI agents. Provides application-facing memory
  APIs and infrastructure for storing, updating, and retrieving user or agent
  memories. Memory type: app/agent memory platform, not codebase search.
- [Hindsight](https://github.com/vectorize-io/hindsight) [![stars](https://img.shields.io/github/stars/vectorize-io/hindsight?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/vectorize-io/hindsight) [![commits](https://img.shields.io/github/commit-activity/m/vectorize-io/hindsight?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/vectorize-io/hindsight): Type: agent memory
  `daemon` `lib`.
  system. Captures, reflects on, and recalls relevant context for future agent
  sessions. Memory type: external extracted memory with recall controls.
- [claude-mem](https://github.com/thedotmack/claude-mem) [![stars](https://img.shields.io/github/stars/thedotmack/claude-mem?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/thedotmack/claude-mem) [![commits](https://img.shields.io/github/commit-activity/m/thedotmack/claude-mem?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/thedotmack/claude-mem): Type: persistent
  `plugin` `daemon`.
  context helper for coding agents. Captures session activity, compresses it,
  and injects relevant context into later sessions. Memory type: extracted
  session memory. Token note: avoid running it beside another recall injector
  without measuring duplicate context.
- [EverOS](https://github.com/EverMind-AI/EverOS) [![stars](https://img.shields.io/github/stars/EverMind-AI/EverOS?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/EverMind-AI/EverOS) [![commits](https://img.shields.io/github/commit-activity/m/EverMind-AI/EverOS?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/EverMind-AI/EverOS): Type: portable memory layer
  `plugin` `daemon`.
  for AI agents. Provides local-first, Markdown-native, user-owned memory across
  apps, tools, and workflows. Memory type: portable long-term agent memory.
- [OKF specification](https://github.com/GoogleCloudPlatform/knowledge-catalog) [![stars](https://img.shields.io/github/stars/GoogleCloudPlatform/knowledge-catalog?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/GoogleCloudPlatform/knowledge-catalog) [![commits](https://img.shields.io/github/commit-activity/m/GoogleCloudPlatform/knowledge-catalog?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/GoogleCloudPlatform/knowledge-catalog):
  `daemon` `plugin` `lib`.
  Type: open knowledge format and catalog repository. Provides a portable
  markdown knowledge-bundle format. Memory type: curated durable knowledge
  format, not a daemon or recall engine. Token note: saves tokens when docs are
  pre-shaped into compact, reusable knowledge files.
- [MemOS](https://github.com/MemTensor/MemOS) [![stars](https://img.shields.io/github/stars/MemTensor/MemOS?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/MemTensor/MemOS) [![commits](https://img.shields.io/github/commit-activity/m/MemTensor/MemOS?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/MemTensor/MemOS): Type: memory operating-system
  `daemon` `lib`.
  research/project. Explores memory lifecycle and storage for AI systems.
  Memory type: research-oriented agent memory layer.

[Back to top](#awesome-ai)

## RAG And Documentation Retrieval

- [Ory Lumen](https://github.com/ory/lumen) [![stars](https://img.shields.io/github/stars/ory/lumen?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ory/lumen) [![commits](https://img.shields.io/github/commit-activity/m/ory/lumen?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ory/lumen): Type: semantic-search MCP/skill
  `mcp` `skill` `lib`.
  layer. Uses embeddings plus local storage to retrieve relevant code/docs for
  agents. RAG type: local semantic index backed by embeddings and SQLite with
  Ollama or LM Studio. Token note: can save tokens by retrieving focused
  context instead of reading broad files, but overlaps with exact search and
  symbol tools.
- [LightRAG](https://github.com/HKUDS/LightRAG) [![stars](https://img.shields.io/github/stars/HKUDS/LightRAG?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/HKUDS/LightRAG) [![commits](https://img.shields.io/github/commit-activity/m/HKUDS/LightRAG?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/HKUDS/LightRAG): Type: retrieval-augmented
  `plugin` `sdk` `daemon` `lib`.
  generation framework. Implements graph-enhanced RAG for simple and fast
  retrieval over documents. RAG type: knowledge-graph/vector retrieval layer.
  Token note: saves context when retrieval returns the small evidence set needed
  for an answer instead of loading the full corpus.
- [LlamaIndex](https://github.com/run-llama/llama_index) [![stars](https://img.shields.io/github/stars/run-llama/llama_index?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/run-llama/llama_index) [![commits](https://img.shields.io/github/commit-activity/m/run-llama/llama_index?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/run-llama/llama_index): Type:
  `sdk` `lib` `daemon`.
  data framework for LLM applications. Connects documents, APIs, structured
  data, indexes, retrievers, and agents for RAG-heavy systems.
- [Haystack](https://github.com/deepset-ai/haystack) [![stars](https://img.shields.io/github/stars/deepset-ai/haystack?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/deepset-ai/haystack) [![commits](https://img.shields.io/github/commit-activity/m/deepset-ai/haystack?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/deepset-ai/haystack): Type:
  `sdk` `daemon` `lib`.
  mature RAG and search pipeline framework. Builds retrieval, ranking,
  generation, evaluation, and production search workflows.
- [DeepWiki Open](https://github.com/AsyncFuncAI/deepwiki-open) [![stars](https://img.shields.io/github/stars/AsyncFuncAI/deepwiki-open?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/AsyncFuncAI/deepwiki-open) [![commits](https://img.shields.io/github/commit-activity/m/AsyncFuncAI/deepwiki-open?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/AsyncFuncAI/deepwiki-open): Type:
  `lib` `sdk`.
  repository documentation/RAG system. Generates or serves explanatory
  repository docs for agent and human consumption. RAG note: codebase
  explanation and retrieval layer; freshness depends on ingestion.
- [Context7](https://github.com/upstash/context7) [![stars](https://img.shields.io/github/stars/upstash/context7?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/upstash/context7) [![commits](https://img.shields.io/github/commit-activity/m/upstash/context7?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/upstash/context7): Type: documentation MCP
  `daemon` `mcp` `sdk` `lib`.
  server. Retrieves current library/framework docs for coding agents. RAG note:
  external documentation retrieval, not persistent memory. Token note: saves
  context by loading targeted docs instead of web dumps.
- [Open Notebook](https://github.com/lfnovo/open-notebook) [![stars](https://img.shields.io/github/stars/lfnovo/open-notebook?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/lfnovo/open-notebook) [![commits](https://img.shields.io/github/commit-activity/m/lfnovo/open-notebook?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/lfnovo/open-notebook): Type:
  `lib`.
  open-source NotebookLM-style knowledge workspace. Lets users ingest,
  organize, query, and work with documents through a flexible local-first
  notebook interface.
- [Firecrawl](https://github.com/firecrawl/firecrawl) [![stars](https://img.shields.io/github/stars/firecrawl/firecrawl?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/firecrawl/firecrawl) [![commits](https://img.shields.io/github/commit-activity/m/firecrawl/firecrawl?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/firecrawl/firecrawl): Type:
  `lib` `daemon`.
  web search, scraping, crawling, and extraction platform. Useful for turning
  web pages into LLM-ready Markdown or structured data for research and RAG
  ingestion. License note: AGPL; review before embedding in proprietary stacks.
- [MarkItDown](https://github.com/microsoft/markitdown) [![stars](https://img.shields.io/github/stars/microsoft/markitdown?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/microsoft/markitdown) [![commits](https://img.shields.io/github/commit-activity/m/microsoft/markitdown?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/microsoft/markitdown): Type:
  `daemon` `lib` `sdk`.
  document-to-Markdown conversion tool. Converts PDFs, Office files, images,
  audio metadata, and other inputs into prompt-friendly Markdown for retrieval
  and agent workflows.
- [Gitingest](https://github.com/coderamp-labs/gitingest) [![stars](https://img.shields.io/github/stars/coderamp-labs/gitingest?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/coderamp-labs/gitingest) [![commits](https://img.shields.io/github/commit-activity/m/coderamp-labs/gitingest?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/coderamp-labs/gitingest): Type:
  `lib` `sdk`.
  prompt-friendly codebase extraction tool. Converts GitHub repositories or
  local source trees into compact text bundles for model context, review, and
  analysis.
- [Sourcebot](https://github.com/sourcebot-dev/sourcebot) [![stars](https://img.shields.io/github/stars/sourcebot-dev/sourcebot?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/sourcebot-dev/sourcebot) [![commits](https://img.shields.io/github/commit-activity/m/sourcebot-dev/sourcebot?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/sourcebot-dev/sourcebot): Type: self-hosted
  `daemon` `lib` `sdk`.
  code search web app. Indexes many repositories for org-scale source search.
  RAG note: retrieval over source repositories, not personal memory. Token note:
  saves agent context when humans or agents can locate the exact files first.
- [Onyx](https://github.com/onyx-dot-app/onyx) [![stars](https://img.shields.io/github/stars/onyx-dot-app/onyx?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/onyx-dot-app/onyx) [![commits](https://img.shields.io/github/commit-activity/m/onyx-dot-app/onyx?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/onyx-dot-app/onyx): Type:
  `daemon` `lib` `sdk`.
  workplace AI search and assistant platform. Connects to team docs and apps
  for shared organizational retrieval. Memory type: shared/team knowledge
  retrieval, not private conversation memory.
- [ParadeDB](https://github.com/paradedb/paradedb) [![stars](https://img.shields.io/github/stars/paradedb/paradedb?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/paradedb/paradedb) [![commits](https://img.shields.io/github/commit-activity/m/paradedb/paradedb?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/paradedb/paradedb): Type:
  `plugin` `lib` `sdk`.
  Postgres search extension with BM25 scoring. RAG type: keyword/BM25 lexical
  retrieval over structured data. Token note: complements embeddings when exact
  terms and filters should retrieve the narrow evidence set.
- [BM25S](https://github.com/xhluca/bm25s) [![stars](https://img.shields.io/github/stars/xhluca/bm25s?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/xhluca/bm25s) [![commits](https://img.shields.io/github/commit-activity/m/xhluca/bm25s?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/xhluca/bm25s): Type: Python
  `sdk` `lib` `daemon`.
  BM25 retrieval library. RAG type: local keyword/BM25 lexical retrieval.
  Token note: useful for cheap first-pass retrieval before vector search or LLM
  ranking.
- [Agent-Reach](https://github.com/Panniantong/Agent-Reach) [![stars](https://img.shields.io/github/stars/Panniantong/Agent-Reach?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Panniantong/Agent-Reach) [![commits](https://img.shields.io/github/commit-activity/m/Panniantong/Agent-Reach?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Panniantong/Agent-Reach): Type: research
  `daemon` `lib` `sdk`.
  connector installer/router. Connects agents to web, YouTube, RSS, GitHub,
  social, and search sources. RAG note: current external research retrieval,
  not durable memory.

[Back to top](#awesome-ai)

## Vector Stores And Retrieval Infrastructure

- [Qdrant](https://github.com/qdrant/qdrant) [![stars](https://img.shields.io/github/stars/qdrant/qdrant?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/qdrant/qdrant) [![commits](https://img.shields.io/github/commit-activity/m/qdrant/qdrant?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/qdrant/qdrant):
  `lib` `daemon` `sdk`.
  Type: dedicated vector database and similarity-search engine. Good default
  when an AI stack needs a simple standalone vector store instead of embedding
  retrieval into an existing application database.
- [pgvector](https://github.com/pgvector/pgvector) [![stars](https://img.shields.io/github/stars/pgvector/pgvector?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/pgvector/pgvector) [![commits](https://img.shields.io/github/commit-activity/m/pgvector/pgvector?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/pgvector/pgvector):
  `plugin` `lib` `daemon`.
  Type: Postgres vector extension. Best default when Postgres already exists
  and vector search should live beside transactional data, metadata filters,
  permissions, and backups.
- [Chroma](https://github.com/chroma-core/chroma) [![stars](https://img.shields.io/github/stars/chroma-core/chroma?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/chroma-core/chroma) [![commits](https://img.shields.io/github/commit-activity/m/chroma-core/chroma?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/chroma-core/chroma):
  `daemon` `lib` `sdk`.
  Type: open-source embedding database. Useful for local AI app development and
  Python-centric retrieval workflows. Stack note: pick one vector store per
  stack unless there is a clear migration or isolation reason.
- [Milvus](https://github.com/milvus-io/milvus) [![stars](https://img.shields.io/github/stars/milvus-io/milvus?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/milvus-io/milvus) [![commits](https://img.shields.io/github/commit-activity/m/milvus-io/milvus?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/milvus-io/milvus):
  `daemon` `lib`.
  Type: distributed vector database. Useful when scale and vector-search
  service separation matter more than operational simplicity.
- [Weaviate](https://github.com/weaviate/weaviate) [![stars](https://img.shields.io/github/stars/weaviate/weaviate?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/weaviate/weaviate) [![commits](https://img.shields.io/github/commit-activity/m/weaviate/weaviate?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/weaviate/weaviate):
  `lib` `daemon` `sdk`.
  Type: vector database and search platform. Useful as an alternative
  retrieval backend with schema, hybrid search, and application-facing APIs.

[Back to top](#awesome-ai)

## Token-Saving Search And Code Intelligence

- [ripgrep](https://github.com/BurntSushi/ripgrep) [![stars](https://img.shields.io/github/stars/BurntSushi/ripgrep?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/BurntSushi/ripgrep) [![commits](https://img.shields.io/github/commit-activity/m/BurntSushi/ripgrep?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/BurntSushi/ripgrep): Type: CLI text search
  `cli` `lib`.
  tool. Fast exact search over local files. Token note: saves context by
  locating exact matches before reading files.
- [fd](https://github.com/sharkdp/fd) [![stars](https://img.shields.io/github/stars/sharkdp/fd?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/sharkdp/fd) [![commits](https://img.shields.io/github/commit-activity/m/sharkdp/fd?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/sharkdp/fd): Type: CLI file finder. Finds candidate
  `cli` `lib`.
  files quickly before content reads. Token note: saves context by narrowing
  file scope.
- [ast-grep](https://github.com/ast-grep/ast-grep) [![stars](https://img.shields.io/github/stars/ast-grep/ast-grep?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ast-grep/ast-grep) [![commits](https://img.shields.io/github/commit-activity/m/ast-grep/ast-grep?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ast-grep/ast-grep): Type: syntax-aware search
  `cli` `lib`.
  and rewrite CLI. Finds imports, functions, hooks, classes, and call shapes.
  Token note: saves context by matching AST structure instead of reading broad
  files.
- [Serena](https://github.com/oraios/serena) [![stars](https://img.shields.io/github/stars/oraios/serena?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/oraios/serena) [![commits](https://img.shields.io/github/commit-activity/m/oraios/serena?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/oraios/serena): Type: coding-agent toolkit and
  `daemon` `mcp` `plugin` `sdk` `lib`.
  MCP server. Provides semantic code navigation, symbol lookup, references,
  call-graph style exploration, and targeted edits. Token note: reduces broad
  file reads by retrieving symbols and relationships directly.
- [FFF](https://github.com/dmtrKovalenko/fff) [![stars](https://img.shields.io/github/stars/dmtrKovalenko/fff?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/dmtrKovalenko/fff) [![commits](https://img.shields.io/github/commit-activity/m/dmtrKovalenko/fff?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/dmtrKovalenko/fff): Type: fast file/content search
  `daemon` `mcp` `plugin` `lib`.
  tool, MCP server, Pi extension, and Neovim plugin. Uses frecency and fuzzy
  fallback for repeated large-repo exploration. Token note: saves tokens when
  fuzzy/frecency search prevents repeated broad `rg`/file reads.
- [Semgrep](https://github.com/semgrep/semgrep) [![stars](https://img.shields.io/github/stars/semgrep/semgrep?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/semgrep/semgrep) [![commits](https://img.shields.io/github/commit-activity/m/semgrep/semgrep?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/semgrep/semgrep): Type: static-analysis and
  `cli` `lib`.
  structural-search CLI/platform. Useful for deterministic security and code
  pattern searches. Token note: produces focused findings instead of broad
  manual inspection.
- [RTK](https://github.com/rtk-ai/rtk) [![stars](https://img.shields.io/github/stars/rtk-ai/rtk?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/rtk-ai/rtk) [![commits](https://img.shields.io/github/commit-activity/m/rtk-ai/rtk?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/rtk-ai/rtk): Type: CLI proxy for reducing noisy shell
  `cli`.
  output before it reaches an LLM. Token note: compresses common development
  command output and should be measured with `rtk gain`.
- [Headroom](https://github.com/headroomlabs-ai/headroom) [![stars](https://img.shields.io/github/stars/headroomlabs-ai/headroom?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/headroomlabs-ai/headroom) [![commits](https://img.shields.io/github/commit-activity/m/headroomlabs-ai/headroom?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/headroomlabs-ai/headroom): Type: library, proxy,
  `daemon` `mcp` `sdk` `lib`.
  and MCP server for context compression. Compresses tool outputs, logs, files,
  and RAG chunks before they reach the LLM.
- [LLMLingua](https://github.com/microsoft/LLMLingua) [![stars](https://img.shields.io/github/stars/microsoft/LLMLingua?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/microsoft/LLMLingua) [![commits](https://img.shields.io/github/commit-activity/m/microsoft/LLMLingua?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/microsoft/LLMLingua): Type:
  `sdk` `lib` `daemon`.
  prompt-compression toolkit. Token-saving type: semantic compression and
  context summarization for prompts, retrieved chunks, and long inputs.
- [GPTCache](https://github.com/zilliztech/GPTCache) [![stars](https://img.shields.io/github/stars/zilliztech/GPTCache?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/zilliztech/GPTCache) [![commits](https://img.shields.io/github/commit-activity/m/zilliztech/GPTCache?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/zilliztech/GPTCache): Type:
  `lib` `daemon` `sdk`.
  semantic cache for LLM applications. Token-saving type: caching repeated or
  similar prompts, responses, embeddings, and retrieval results.

[Back to top](#awesome-ai)

## Structured Outputs

- [Outlines](https://github.com/dottxt-ai/outlines) [![stars](https://img.shields.io/github/stars/dottxt-ai/outlines?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/dottxt-ai/outlines) [![commits](https://img.shields.io/github/commit-activity/m/dottxt-ai/outlines?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/dottxt-ai/outlines): Type:
  `sdk` `daemon` `lib`.
  constrained generation library. Token-saving type: structured outputs that
  reduce retries, parsing chatter, and invalid JSON/schema responses.
- [Instructor](https://github.com/instructor-ai/instructor) [![stars](https://img.shields.io/github/stars/instructor-ai/instructor?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/instructor-ai/instructor) [![commits](https://img.shields.io/github/commit-activity/m/instructor-ai/instructor?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/instructor-ai/instructor): Type:
  `sdk` `daemon` `lib`.
  structured output and extraction library. Token-saving type: structured
  outputs with schema validation, retries, and typed extraction.

[Back to top](#awesome-ai)

## MCP, Connectors, And Protocols

- [Model Context Protocol](https://github.com/modelcontextprotocol/modelcontextprotocol) [![stars](https://img.shields.io/github/stars/modelcontextprotocol/modelcontextprotocol?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/modelcontextprotocol/modelcontextprotocol) [![commits](https://img.shields.io/github/commit-activity/m/modelcontextprotocol/modelcontextprotocol?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/modelcontextprotocol/modelcontextprotocol):
  `mcp` `sdk` `daemon` `lib`.
  Type: open protocol/specification plus SDK ecosystem. Standardizes how LLM
  clients connect to tools, data sources, prompts, and resources. RAG note:
  connector protocol for live retrieval/tool use, not memory by itself.
- [MCP reference servers](https://github.com/modelcontextprotocol/servers) [![stars](https://img.shields.io/github/stars/modelcontextprotocol/servers?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/modelcontextprotocol/servers) [![commits](https://img.shields.io/github/commit-activity/m/modelcontextprotocol/servers?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/modelcontextprotocol/servers):
  `daemon` `mcp` `plugin` `sdk` `lib`.
  Type: MCP server implementations. Provides connector examples for services
  and local resources. Token note: can save prompt tokens by fetching focused
  external context on demand, but tool schemas add overhead when enabled
  globally.
- [FastMCP](https://github.com/PrefectHQ/fastmcp) [![stars](https://img.shields.io/github/stars/PrefectHQ/fastmcp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/PrefectHQ/fastmcp) [![commits](https://img.shields.io/github/commit-activity/m/PrefectHQ/fastmcp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/PrefectHQ/fastmcp): Type:
  `daemon` `mcp` `sdk`.
  Python framework for building MCP servers and clients. Useful for exposing
  local services, APIs, prompts, resources, and tools through MCP.
- [MCP-Github-Agent / Code2MCP](https://github.com/DEFENSE-SEU/MCP-Github-Agent) [![stars](https://img.shields.io/github/stars/DEFENSE-SEU/MCP-Github-Agent?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/DEFENSE-SEU/MCP-Github-Agent) [![commits](https://img.shields.io/github/commit-activity/m/DEFENSE-SEU/MCP-Github-Agent?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/DEFENSE-SEU/MCP-Github-Agent):
  `daemon` `mcp` `sdk` `lib`.
  Type: multi-agent MCP generation framework. Converts GitHub repositories into
  MCP services through automated analysis, generation, run, review, and fix
  loops. RAG note: turns code repositories into tool/context services rather
  than storing personal memory.
- [mcp-use](https://github.com/mcp-use/mcp-use) [![stars](https://img.shields.io/github/stars/mcp-use/mcp-use?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mcp-use/mcp-use) [![commits](https://img.shields.io/github/commit-activity/m/mcp-use/mcp-use?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mcp-use/mcp-use): Type:
  `daemon` `mcp` `sdk`.
  full-stack MCP framework. Helps build MCP apps and agents that consume MCP
  servers instead of only defining new servers.
- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) [![stars](https://img.shields.io/github/stars/punkpeye/awesome-mcp-servers?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/punkpeye/awesome-mcp-servers) [![commits](https://img.shields.io/github/commit-activity/m/punkpeye/awesome-mcp-servers?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/punkpeye/awesome-mcp-servers): Type:
  `daemon` `mcp`.
  MCP server directory. Curates community MCP servers by category so agents can
  discover connector options without enabling every server globally.
- [mcp-server-bash-sdk](https://github.com/muthuishere/mcp-server-bash-sdk) [![stars](https://img.shields.io/github/stars/muthuishere/mcp-server-bash-sdk?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/muthuishere/mcp-server-bash-sdk) [![commits](https://img.shields.io/github/commit-activity/m/muthuishere/mcp-server-bash-sdk?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/muthuishere/mcp-server-bash-sdk):
  `cli` `daemon` `mcp` `sdk`.
  Type: Bash SDK/reference for MCP servers. Useful for small local MCP tools and
  shell-backed connector experiments.
- [tmux MCP](https://github.com/nickgnd/tmux-mcp) [![stars](https://img.shields.io/github/stars/nickgnd/tmux-mcp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/nickgnd/tmux-mcp) [![commits](https://img.shields.io/github/commit-activity/m/nickgnd/tmux-mcp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/nickgnd/tmux-mcp): Type: MCP server for tmux.
  `cli` `daemon` `mcp`.
  Lets an agent inspect or control terminal multiplexer sessions. Runtime note:
  broad terminal control is powerful and should be enabled only with a clear
  task and permission boundary.
- [3GPP MCP](https://github.com/higebu/3gpp-mcp) [![stars](https://img.shields.io/github/stars/higebu/3gpp-mcp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/higebu/3gpp-mcp) [![commits](https://img.shields.io/github/commit-activity/m/higebu/3gpp-mcp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/higebu/3gpp-mcp): Type: MCP server for 3GPP
  `daemon` `mcp` `lib` `sdk`.
  specification access. Useful for telecom agents that need focused retrieval
  over 3GPP material.
- [GitHub MCP server](https://github.com/github/github-mcp-server) [![stars](https://img.shields.io/github/stars/github/github-mcp-server?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/github/github-mcp-server) [![commits](https://img.shields.io/github/commit-activity/m/github/github-mcp-server?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/github/github-mcp-server): Type:
  `daemon` `mcp`.
  GitHub connector MCP server. Lets agents inspect or update GitHub issues,
  PRs, files, and repo metadata when scoped credentials are available.
- [Atlassian MCP server](https://github.com/sooperset/mcp-atlassian) [![stars](https://img.shields.io/github/stars/sooperset/mcp-atlassian?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/sooperset/mcp-atlassian) [![commits](https://img.shields.io/github/commit-activity/m/sooperset/mcp-atlassian?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/sooperset/mcp-atlassian): Type:
  `daemon` `mcp` `lib`.
  Jira/Confluence connector MCP server. Lets agents read and update Atlassian
  work items or documentation.
- [Agent2Agent / A2A](https://github.com/a2aproject/A2A) [![stars](https://img.shields.io/github/stars/a2aproject/A2A?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/a2aproject/A2A) [![commits](https://img.shields.io/github/commit-activity/m/a2aproject/A2A?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/a2aproject/A2A): Type:
  `mcp` `lib`.
  agent-to-agent protocol/specification. Uses agent cards, tasks, streaming,
  push notifications, and auth/security objects for cross-agent
  interoperability.

[Back to top](#awesome-ai)

## Task Management

- [Beads](https://github.com/gastownhall/beads) [![stars](https://img.shields.io/github/stars/gastownhall/beads?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/gastownhall/beads) [![commits](https://img.shields.io/github/commit-activity/m/gastownhall/beads?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/gastownhall/beads): Type: distributed graph issue
  `cli` `daemon` `lib`.
  tracker CLI for AI agents. Uses Dolt-backed storage, dependency tracking,
  ready-task selection, atomic claim/update flow, JSON output, and project
  memory. Memory type: project task memory, not chat memory. Token note: saves
  context in multi-agent repos by making the next unblocked work queryable.
- [Task Master](https://github.com/eyaltoledano/claude-task-master) [![stars](https://img.shields.io/github/stars/eyaltoledano/claude-task-master?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/eyaltoledano/claude-task-master) [![commits](https://img.shields.io/github/commit-activity/m/eyaltoledano/claude-task-master?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/eyaltoledano/claude-task-master): Type: AI
  `cli` `mcp` `lib`.
  task manager CLI/MCP. Parses PRDs, expands tasks, tracks dependencies, and
  offers next-task/research commands. Token note: supports reduced MCP tool
  modes such as `core` or `standard` to avoid loading the full tool surface.
- [Workstream](https://github.com/happybhati/workstream) [![stars](https://img.shields.io/github/stars/happybhati/workstream?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/happybhati/workstream) [![commits](https://img.shields.io/github/commit-activity/m/happybhati/workstream?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/happybhati/workstream): Type: task/workflow
  `daemon` `cli` `lib`.
  dashboard. Tracked as a possible broader work queue UI when simple local
  state fragments.
- [Taskwarrior](https://github.com/GothenburgBitFactory/taskwarrior) [![stars](https://img.shields.io/github/stars/GothenburgBitFactory/taskwarrior?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/GothenburgBitFactory/taskwarrior) [![commits](https://img.shields.io/github/commit-activity/m/GothenburgBitFactory/taskwarrior?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/GothenburgBitFactory/taskwarrior): Type:
  `cli`.
  personal task CLI. Useful for human offline GTD-style task tracking; weaker
  for multi-agent sync unless paired with a deliberate sync process.

[Back to top](#awesome-ai)

## Workflow Orchestration

- [Codex-Workflows](https://github.com/robzilla1738/Codex-Workflows) [![stars](https://img.shields.io/github/stars/robzilla1738/Codex-Workflows?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/robzilla1738/Codex-Workflows) [![commits](https://img.shields.io/github/commit-activity/m/robzilla1738/Codex-Workflows?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/robzilla1738/Codex-Workflows): Type:
  `cli` `daemon` `mcp` `plugin`.
  Codex plugin, MCP server, and TUI workflow-as-code runner. Runs trusted
  workflow definitions for bug sweeps, release diff review, auth/security
  review, and other repeatable processes.
- [CC Workflow Studio](https://github.com/breaking-brake/cc-wf-studio) [![stars](https://img.shields.io/github/stars/breaking-brake/cc-wf-studio?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/breaking-brake/cc-wf-studio) [![commits](https://img.shields.io/github/commit-activity/m/breaking-brake/cc-wf-studio?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/breaking-brake/cc-wf-studio): Type:
  `plugin` `daemon`.
  Claude Code workflow studio. Provides a workflow-oriented interface for
  designing, managing, and running Claude Code automation patterns.
- [OpenSpec](https://github.com/Fission-AI/OpenSpec) [![stars](https://img.shields.io/github/stars/Fission-AI/OpenSpec?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Fission-AI/OpenSpec) [![commits](https://img.shields.io/github/commit-activity/m/Fission-AI/OpenSpec?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Fission-AI/OpenSpec): Type:
  `daemon`.
  spec-driven development tool for AI coding assistants. Helps turn specs into
  structured implementation context, tasks, and agent-ready development flows.
- [PilotDeck](https://github.com/OpenBMB/PilotDeck) [![stars](https://img.shields.io/github/stars/OpenBMB/PilotDeck?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/OpenBMB/PilotDeck) [![commits](https://img.shields.io/github/commit-activity/m/OpenBMB/PilotDeck?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/OpenBMB/PilotDeck): Type: agent build/deploy
  `daemon`.
  workflow project. Tracked as a deployment workflow reference.
- [AgentWrapper orchestrator](https://github.com/AgentWrapper/agent-orchestrator) [![stars](https://img.shields.io/github/stars/AgentWrapper/agent-orchestrator?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/AgentWrapper/agent-orchestrator) [![commits](https://img.shields.io/github/commit-activity/m/AgentWrapper/agent-orchestrator?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/AgentWrapper/agent-orchestrator):
  `daemon` `sdk`.
  Type: agent orchestration framework. Tracked as a reference for coordinating
  agents rather than a default local runtime.
- [n8n](https://github.com/n8n-io/n8n) [![stars](https://img.shields.io/github/stars/n8n-io/n8n?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/n8n-io/n8n) [![commits](https://img.shields.io/github/commit-activity/m/n8n-io/n8n?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/n8n-io/n8n): Type:
  `plugin` `daemon`.
  workflow automation platform. Provides practical automation glue, API
  integrations, triggers, and human-readable workflows that can replace custom
  agent orchestration code for many operational tasks.
- [Clawpatch](https://github.com/openclaw/clawpatch) [![stars](https://img.shields.io/github/stars/openclaw/clawpatch?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openclaw/clawpatch) [![commits](https://img.shields.io/github/commit-activity/m/openclaw/clawpatch?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openclaw/clawpatch): Type: code review and
  `daemon`.
  patch workflow tool. Reviews code, patches bugs, and helps land PRs.
- [Lobster](https://github.com/openclaw/lobster) [![stars](https://img.shields.io/github/stars/openclaw/lobster?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openclaw/lobster) [![commits](https://img.shields.io/github/commit-activity/m/openclaw/lobster?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openclaw/lobster): Type: OpenClaw-native
  `cli` `skill` `daemon`.
  workflow shell. Turns skills and tools into typed, local-first pipelines and
  safe automations callable from OpenClaw.
- [Babysitter](https://github.com/a5c-ai/babysitter) [![stars](https://img.shields.io/github/stars/a5c-ai/babysitter?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/a5c-ai/babysitter) [![commits](https://img.shields.io/github/commit-activity/m/a5c-ai/babysitter?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/a5c-ai/babysitter): Type: SDK, CLI, MCP
  `cli` `daemon` `mcp` `plugin`.
  server, and plugin for code-defined agent workflows. Provides harness
  discovery, approvals, journaling, and runner abstraction. Runtime note:
  useful when hard sequencing and approval gates are worth a separate workflow
  layer.
- [Temporal](https://github.com/temporalio/temporal) [![stars](https://img.shields.io/github/stars/temporalio/temporal?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/temporalio/temporal) [![commits](https://img.shields.io/github/commit-activity/m/temporalio/temporal?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/temporalio/temporal): Type:
  `daemon`.
  durable workflow orchestration service. Provides long-running workflow state,
  retries, timers, signals, and activity execution for agentic systems that
  need reliable background work. Memory type: event-sourced workflow state, not
  semantic agent memory.
- [Compound Engineering plugin](https://github.com/EveryInc/compound-engineering-plugin) [![stars](https://img.shields.io/github/stars/EveryInc/compound-engineering-plugin?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/EveryInc/compound-engineering-plugin) [![commits](https://img.shields.io/github/commit-activity/m/EveryInc/compound-engineering-plugin?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/EveryInc/compound-engineering-plugin):
  `plugin` `skill` `daemon`.
  Type: planning, review, and compound-learning plugin/skill set. Useful for
  structured strategy and review cycles when its opinionated workflow beats
  local skills.
- [autoresearch](https://github.com/karpathy/autoresearch) [![stars](https://img.shields.io/github/stars/karpathy/autoresearch?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/karpathy/autoresearch) [![commits](https://img.shields.io/github/commit-activity/m/karpathy/autoresearch?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/karpathy/autoresearch): Type: autonomous
  `daemon` `lib`.
  research-loop experiment. Reference for research loop design and bounded
  iteration.

[Back to top](#awesome-ai)

## Skills And Agent Packs

- [Agent Skills](https://github.com/scienceaix/agentskills) [![stars](https://img.shields.io/github/stars/scienceaix/agentskills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/scienceaix/agentskills) [![commits](https://img.shields.io/github/commit-activity/m/scienceaix/agentskills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/scienceaix/agentskills): Type: open skill
  `skill`.
  package specification and examples. Defines `SKILL.md`, metadata, optional
  scripts, references, assets, progressive disclosure, and validation. Token
  note: skills save prompt tokens by exposing compact metadata first and loading
  full instructions only when relevant.
- [OpenClaw agent skills](https://github.com/openclaw/agent-skills) [![stars](https://img.shields.io/github/stars/openclaw/agent-skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/openclaw/agent-skills) [![commits](https://img.shields.io/github/commit-activity/m/openclaw/agent-skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/openclaw/agent-skills): Type:
  `skill` `daemon`.
  shared skill pack for OpenClaw-compatible agents. Includes review, handoff,
  transcript, session-viewer, and remote-proof style workflows. Token note:
  skill metadata is lightweight; full instructions load only when selected.
- [steipete agent scripts](https://github.com/steipete/agent-scripts) [![stars](https://img.shields.io/github/stars/steipete/agent-scripts?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/steipete/agent-scripts) [![commits](https://img.shields.io/github/commit-activity/m/steipete/agent-scripts?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/steipete/agent-scripts): Type:
  `skill` `daemon`.
  agent skill and script collection. Includes maintainer orchestration and
  GitHub project triage patterns.
- [awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) [![stars](https://img.shields.io/github/stars/VoltAgent/awesome-claude-code-subagents?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/VoltAgent/awesome-claude-code-subagents) [![commits](https://img.shields.io/github/commit-activity/m/VoltAgent/awesome-claude-code-subagents?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/VoltAgent/awesome-claude-code-subagents):
  `skill` `sdk`.
  Type: curated subagent pattern list. Useful as a discovery source for agent
  roles; install individual agents only after reviewing tool access and prompt
  scope.
- [taste-skill](https://github.com/Leonxlnx/taste-skill) [![stars](https://img.shields.io/github/stars/Leonxlnx/taste-skill?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Leonxlnx/taste-skill) [![commits](https://img.shields.io/github/commit-activity/m/Leonxlnx/taste-skill?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Leonxlnx/taste-skill): Type: agent skill for
  `skill`.
  taste and quality control. Tries to steer agents away from generic output and
  toward more opinionated, polished results.
- [stop-slop](https://github.com/hardikpandya/stop-slop) [![stars](https://img.shields.io/github/stars/hardikpandya/stop-slop?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/hardikpandya/stop-slop) [![commits](https://img.shields.io/github/commit-activity/m/hardikpandya/stop-slop?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/hardikpandya/stop-slop): Type: prose cleanup
  `skill`.
  skill. Helps remove common AI tells from generated writing.
- [Claude Code Templates](https://github.com/davila7/claude-code-templates) [![stars](https://img.shields.io/github/stars/davila7/claude-code-templates?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/davila7/claude-code-templates) [![commits](https://img.shields.io/github/commit-activity/m/davila7/claude-code-templates?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/davila7/claude-code-templates):
  `cli` `skill`.
  Type: CLI and template pack for configuring and monitoring Claude Code.
  Includes templates, commands, agents, and configuration patterns.
- [design.md](https://github.com/google-labs-code/design.md) [![stars](https://img.shields.io/github/stars/google-labs-code/design.md?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/google-labs-code/design.md) [![commits](https://img.shields.io/github/commit-activity/m/google-labs-code/design.md?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/google-labs-code/design.md): Type: design
  `skill` `plugin`.
  system specification for coding agents. Gives agents a persistent structured
  description of visual identity and design-system rules.
- [no-mistakes](https://github.com/kunchenguid/no-mistakes) [![stars](https://img.shields.io/github/stars/kunchenguid/no-mistakes?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/kunchenguid/no-mistakes) [![commits](https://img.shields.io/github/commit-activity/m/kunchenguid/no-mistakes?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/kunchenguid/no-mistakes): Type: Git push
  `skill` `plugin`.
  guard for agent-assisted work. Helps prevent accidental pushes and other
  avoidable mistakes when coding agents make repository changes.
- [Ponytail](https://github.com/DietrichGebert/ponytail) [![stars](https://img.shields.io/github/stars/DietrichGebert/ponytail?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/DietrichGebert/ponytail) [![commits](https://img.shields.io/github/commit-activity/m/DietrichGebert/ponytail?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/DietrichGebert/ponytail): Type:
  `plugin` `skill`.
  minimalism/YAGNI skill and plugin. Includes review commands focused on small,
  non-speculative changes.
- [alexknowshtml Claude skills](https://github.com/alexknowshtml/claude-skills) [![stars](https://img.shields.io/github/stars/alexknowshtml/claude-skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/alexknowshtml/claude-skills) [![commits](https://img.shields.io/github/commit-activity/m/alexknowshtml/claude-skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/alexknowshtml/claude-skills):
  `skill`.
  Type: Claude skill pack. The `teach` skill is a workspace teaching pattern
  reference.
- [Ryan Singer shaping skills](https://github.com/rjs/shaping-skills) [![stars](https://img.shields.io/github/stars/rjs/shaping-skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/rjs/shaping-skills) [![commits](https://img.shields.io/github/commit-activity/m/rjs/shaping-skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/rjs/shaping-skills): Type:
  `skill` `daemon`.
  product-shaping skill pack. Covers Shape Up framing, kickoff, shaping, and
  breadboarding workflows.
- [Matt Pocock skills](https://github.com/mattpocock/skills) [![stars](https://img.shields.io/github/stars/mattpocock/skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mattpocock/skills) [![commits](https://img.shields.io/github/commit-activity/m/mattpocock/skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mattpocock/skills): Type:
  `skill` `lib`.
  engineering skill pack. Includes diagnose, docs-grounded review, triage, TDD,
  issue conversion, and zoom-out patterns.
- [Addy Osmani agent skills](https://github.com/addyosmani/agent-skills) [![stars](https://img.shields.io/github/stars/addyosmani/agent-skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/addyosmani/agent-skills) [![commits](https://img.shields.io/github/commit-activity/m/addyosmani/agent-skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/addyosmani/agent-skills):
  `skill` `daemon`.
  Type: lifecycle skill pack. Covers spec, plan, build, test, review, and ship
  workflows.
- [Karpathy-inspired skills](https://github.com/forrestchang/andrej-karpathy-skills) [![stars](https://img.shields.io/github/stars/forrestchang/andrej-karpathy-skills?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/forrestchang/andrej-karpathy-skills) [![commits](https://img.shields.io/github/commit-activity/m/forrestchang/andrej-karpathy-skills?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/forrestchang/andrej-karpathy-skills):
  `skill`.
  Type: agent behavior skill pack. Encodes caution, simplicity, surgical edits,
  and goal-driven execution patterns.
- [last30days-skill](https://github.com/mvanhorn/last30days-skill) [![stars](https://img.shields.io/github/stars/mvanhorn/last30days-skill?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mvanhorn/last30days-skill) [![commits](https://img.shields.io/github/commit-activity/m/mvanhorn/last30days-skill?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mvanhorn/last30days-skill): Type:
  `skill` `lib`.
  research skill for agents. Searches Reddit, X, YouTube, Hacker News,
  Polymarket, and the web, then synthesizes a grounded recent-context summary.
- [Nightscout CGM skill](https://github.com/shanselman/nightscout-cgm-skill) [![stars](https://img.shields.io/github/stars/shanselman/nightscout-cgm-skill?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/shanselman/nightscout-cgm-skill) [![commits](https://img.shields.io/github/commit-activity/m/shanselman/nightscout-cgm-skill?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/shanselman/nightscout-cgm-skill):
  `skill` `plugin`.
  Type: domain-specific GitHub Copilot agent skill. Provides a skill package for
  Nightscout CGM blood-glucose analysis. Safety note: health-related output
  needs human/domain review before use.

[Back to top](#awesome-ai)

## Browser Automation And Proof

- [Playwright](https://github.com/microsoft/playwright) [![stars](https://img.shields.io/github/stars/microsoft/playwright?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/microsoft/playwright) [![commits](https://img.shields.io/github/commit-activity/m/microsoft/playwright?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/microsoft/playwright): Type: browser
  `sdk` `daemon`.
  automation and testing framework. Useful for agents that need to verify web
  UI behavior across Chromium, Firefox, and WebKit.
- [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) [![stars](https://img.shields.io/github/stars/ChromeDevTools/chrome-devtools-mcp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ChromeDevTools/chrome-devtools-mcp) [![commits](https://img.shields.io/github/commit-activity/m/ChromeDevTools/chrome-devtools-mcp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ChromeDevTools/chrome-devtools-mcp):
  `daemon` `mcp` `sdk`.
  Type: MCP server for Chrome DevTools. Gives coding agents browser inspection
  and debugging capabilities through DevTools.
- [browser-use](https://github.com/browser-use/browser-use) [![stars](https://img.shields.io/github/stars/browser-use/browser-use?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/browser-use/browser-use) [![commits](https://img.shields.io/github/commit-activity/m/browser-use/browser-use?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/browser-use/browser-use): Type:
  `sdk` `daemon`.
  browser-agent framework. Makes websites accessible to AI agents for web task
  automation, extraction, and browser-controlled workflows.
- [Stagehand](https://github.com/browserbase/stagehand) [![stars](https://img.shields.io/github/stars/browserbase/stagehand?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/browserbase/stagehand) [![commits](https://img.shields.io/github/commit-activity/m/browserbase/stagehand?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/browserbase/stagehand): Type:
  `sdk` `daemon`.
  browser-agent SDK. Wraps browser automation in agent-friendly actions,
  extraction, observation, and deterministic control patterns.
- [Proofshot](https://github.com/AmElmo/proofshot) [![stars](https://img.shields.io/github/stars/AmElmo/proofshot?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/AmElmo/proofshot) [![commits](https://img.shields.io/github/commit-activity/m/AmElmo/proofshot?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/AmElmo/proofshot): Type: browser proof and
  `sdk`.
  artifact capture tool for coding agents. Records browser sessions, captures
  screenshots, collects errors, and bundles verification artifacts.

[Back to top](#awesome-ai)

## Web Automation And CLI Generation

- [OpenCLI](https://github.com/jackwener/OpenCLI) [![stars](https://img.shields.io/github/stars/jackwener/OpenCLI?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/jackwener/OpenCLI) [![commits](https://img.shields.io/github/commit-activity/m/jackwener/OpenCLI?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/jackwener/OpenCLI):
  `cli` `daemon` `sdk`.
  Type: website-to-CLI/browser automation tool. Turns websites into command-line
  interfaces for repeatable web tasks, automation, and agent-accessible actions.
  Stack note: useful when a site has no clean API, but do not use it as a
  replacement for Playwright proof or first-party service APIs.
- [Printing Press](https://github.com/mvanhorn/cli-printing-press) [![stars](https://img.shields.io/github/stars/mvanhorn/cli-printing-press?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/mvanhorn/cli-printing-press) [![commits](https://img.shields.io/github/commit-activity/m/mvanhorn/cli-printing-press?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/mvanhorn/cli-printing-press): Type:
  `cli` `daemon` `lib` `sdk`.
  agent-first CLI generator/research workflow. Discovers API capabilities,
  compares competing tools, and builds CLIs with local SQLite sync and offline
  search.

[Back to top](#awesome-ai)

## Voice, Multimodal, And Realtime Agents

- [Pipecat](https://github.com/pipecat-ai/pipecat) [![stars](https://img.shields.io/github/stars/pipecat-ai/pipecat?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/pipecat-ai/pipecat) [![commits](https://img.shields.io/github/commit-activity/m/pipecat-ai/pipecat?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/pipecat-ai/pipecat): Type: Python framework for
  `skill` `sdk` `daemon`.
  realtime voice and multimodal agents. Supports voice pipelines,
  WebRTC/WebSocket transports, multi-agent flows, deployment tooling, and
  skills.
- [Pipecat Flows](https://github.com/pipecat-ai/pipecat-flows) [![stars](https://img.shields.io/github/stars/pipecat-ai/pipecat-flows?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/pipecat-ai/pipecat-flows) [![commits](https://img.shields.io/github/commit-activity/m/pipecat-ai/pipecat-flows?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/pipecat-ai/pipecat-flows):
  `sdk`.
  Type: structured dialog-flow layer for Pipecat. Adds stateful conversation
  flow control when realtime voice agents need deterministic steps, branching,
  and reusable dialog structure.
- [Voicebox](https://github.com/jamiepine/voicebox) [![stars](https://img.shields.io/github/stars/jamiepine/voicebox?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/jamiepine/voicebox) [![commits](https://img.shields.io/github/commit-activity/m/jamiepine/voicebox?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/jamiepine/voicebox): Type:
  `daemon` `sdk`.
  open-source AI voice studio. Supports voice cloning, dictation, creation,
  and studio-style workflows for speech and voice generation.
- [LiveKit Agents](https://github.com/livekit/agents) [![stars](https://img.shields.io/github/stars/livekit/agents?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/livekit/agents) [![commits](https://img.shields.io/github/commit-activity/m/livekit/agents?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/livekit/agents): Type:
  `plugin` `sdk` `daemon`.
  realtime voice and multimodal agent framework. Builds agents for LiveKit
  rooms with speech, video, tools, and low-latency media workflows.
- [LiveKit SIP](https://github.com/livekit/sip) [![stars](https://img.shields.io/github/stars/livekit/sip?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/livekit/sip) [![commits](https://img.shields.io/github/commit-activity/m/livekit/sip?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/livekit/sip): Type:
  `sdk`.
  SIP bridge for LiveKit. Critical for SIP-to-WebRTC voice-agent stacks where
  phone-network calls need to enter LiveKit rooms for realtime agents.
- [LiveKit Egress](https://github.com/livekit/egress) [![stars](https://img.shields.io/github/stars/livekit/egress?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/livekit/egress) [![commits](https://img.shields.io/github/commit-activity/m/livekit/egress?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/livekit/egress): Type:
  `daemon` `sdk`.
  recording and export service for LiveKit rooms. Useful for voice-agent QA,
  transcripts, audits, call replay, training data, and compliance workflows.
- [TEN Framework](https://github.com/TEN-framework/ten-framework) [![stars](https://img.shields.io/github/stars/TEN-framework/ten-framework?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/TEN-framework/ten-framework) [![commits](https://img.shields.io/github/commit-activity/m/TEN-framework/ten-framework?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/TEN-framework/ten-framework):
  `plugin` `sdk`.
  Type: conversational voice AI framework. Provides an all-in-one alternative
  for realtime voice agents and is worth tracking beside Pipecat and LiveKit
  Agents.
- [VoiceBlender](https://github.com/voiceblender/voiceblender) [![stars](https://img.shields.io/github/stars/voiceblender/voiceblender?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/voiceblender/voiceblender) [![commits](https://img.shields.io/github/commit-activity/m/voiceblender/voiceblender?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/voiceblender/voiceblender): Type:
  `daemon` `plugin` `sdk`.
  SIP/WebRTC AI voice framework and service. Provides AI agent, TTS/STT, rooms,
  and webhook ideas for voice-agent systems.
- [Patter](https://github.com/PatterAI/Patter) [![stars](https://img.shields.io/github/stars/PatterAI/Patter?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/PatterAI/Patter) [![commits](https://img.shields.io/github/commit-activity/m/PatterAI/Patter?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/PatterAI/Patter):
  `sdk`.
  Type: open-source voice AI SDK. Tracked as a telephony-friendly voice-agent
  stack with Twilio, Telnyx, and Plivo framing.
- [Ultravox](https://github.com/fixie-ai/ultravox) [![stars](https://img.shields.io/github/stars/fixie-ai/ultravox?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/fixie-ai/ultravox) [![commits](https://img.shields.io/github/commit-activity/m/fixie-ai/ultravox?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/fixie-ai/ultravox):
  `plugin` `sdk`.
  Type: realtime voice model/project reference. Useful for voice-model
  architecture awareness and low-latency speech-to-speech design ideas.
- [Open Floor](https://github.com/open-voice-interoperability) [![stars](https://img.shields.io/github/stars/open-voice-interoperability/openfloor-docs?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/open-voice-interoperability/openfloor-docs) [![commits](https://img.shields.io/github/commit-activity/m/open-voice-interoperability/openfloor-docs?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/open-voice-interoperability/openfloor-docs):
  `plugin` `lib` `sdk`.
  Type: voice-agent interoperability specification family. Low-star but
  relevant reference material for voice-agent handoff, routing, and cross-agent
  protocol ideas.
- [Janus Gateway](https://github.com/meetecho/janus-gateway) [![stars](https://img.shields.io/github/stars/meetecho/janus-gateway?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/meetecho/janus-gateway) [![commits](https://img.shields.io/github/commit-activity/m/meetecho/janus-gateway?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/meetecho/janus-gateway): Type: WebRTC
  `daemon` `sdk`.
  server/gateway. Infrastructure option for realtime AI voice, SIP/WebRTC, and
  multimodal projects.
- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) [![stars](https://img.shields.io/github/stars/ggml-org/whisper.cpp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ggml-org/whisper.cpp) [![commits](https://img.shields.io/github/commit-activity/m/ggml-org/whisper.cpp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ggml-org/whisper.cpp):
  `daemon` `sdk`.
  Type: local and edge speech-to-text inference runtime. Major primitive for
  offline, private, and low-cost STT in voice-agent stacks.
- [faster-whisper](https://github.com/SYSTRAN/faster-whisper) [![stars](https://img.shields.io/github/stars/SYSTRAN/faster-whisper?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/SYSTRAN/faster-whisper) [![commits](https://img.shields.io/github/commit-activity/m/SYSTRAN/faster-whisper?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/SYSTRAN/faster-whisper):
  `sdk` `daemon`.
  Type: faster Whisper inference implementation. Important STT option for
  production and batch workloads; maintenance should be checked before choosing
  it as the default.
- [Silero VAD](https://github.com/snakers4/silero-vad) [![stars](https://img.shields.io/github/stars/snakers4/silero-vad?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/snakers4/silero-vad) [![commits](https://img.shields.io/github/commit-activity/m/snakers4/silero-vad?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/snakers4/silero-vad):
  `sdk`.
  Type: voice activity detection model. Voice stacks need VAD as a first-class
  primitive for turn-taking, latency, interruption handling, and cost control.
- [Kokoro](https://github.com/hexgrad/kokoro) [![stars](https://img.shields.io/github/stars/hexgrad/kokoro?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/hexgrad/kokoro) [![commits](https://img.shields.io/github/commit-activity/m/hexgrad/kokoro?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/hexgrad/kokoro):
  `sdk`.
  Type: local TTS model/project. Useful low-latency local speech synthesis
  candidate; verify current maintenance and model quality before production
  adoption.
- [audio.cpp](https://github.com/0xShug0/audio.cpp) [![stars](https://img.shields.io/github/stars/0xShug0/audio.cpp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/0xShug0/audio.cpp) [![commits](https://img.shields.io/github/commit-activity/m/0xShug0/audio.cpp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/0xShug0/audio.cpp): Type: C++ inference engine
  `sdk` `daemon`.
  for audio models. Supports STT, TTS, VAD, voice conversion, music generation,
  and other audio-model workloads. License note: repository LICENSE is Apache
  2.0, although GitHub classifies it as `Other`.

[Back to top](#awesome-ai)

## Local Model Runtimes And App Platforms

- [Ollama](https://github.com/ollama/ollama) [![stars](https://img.shields.io/github/stars/ollama/ollama?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ollama/ollama) [![commits](https://img.shields.io/github/commit-activity/m/ollama/ollama?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ollama/ollama): Type:
  `daemon`.
  local model runtime. Runs and serves local LLMs with a simple developer
  workflow and broad ecosystem support.
- [llama.cpp](https://github.com/ggml-org/llama.cpp) [![stars](https://img.shields.io/github/stars/ggml-org/llama.cpp?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/ggml-org/llama.cpp) [![commits](https://img.shields.io/github/commit-activity/m/ggml-org/llama.cpp?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/ggml-org/llama.cpp): Type:
  `daemon` `plugin`.
  local and edge inference runtime. Provides efficient CPU/GPU inference for
  GGUF models and underpins many local-model tools.
- [vLLM](https://github.com/vllm-project/vllm) [![stars](https://img.shields.io/github/stars/vllm-project/vllm?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/vllm-project/vllm) [![commits](https://img.shields.io/github/commit-activity/m/vllm-project/vllm?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/vllm-project/vllm): Type:
  `daemon` `plugin`.
  server inference runtime. Provides high-throughput model serving, OpenAI API
  compatibility patterns, batching, and production-oriented deployment support.
- [Open WebUI](https://github.com/open-webui/open-webui) [![stars](https://img.shields.io/github/stars/open-webui/open-webui?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/open-webui/open-webui) [![commits](https://img.shields.io/github/commit-activity/m/open-webui/open-webui?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/open-webui/open-webui): Type:
  `daemon` `lib` `sdk`.
  local AI web UI. Common self-hosted interface for Ollama, OpenAI-compatible
  APIs, tools, retrieval, and personal/team AI workflows.
- [Langflow](https://github.com/langflow-ai/langflow) [![stars](https://img.shields.io/github/stars/langflow-ai/langflow?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langflow-ai/langflow) [![commits](https://img.shields.io/github/commit-activity/m/langflow-ai/langflow?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langflow-ai/langflow): Type:
  `plugin` `lib` `daemon` `sdk`.
  visual agent and RAG builder. Provides low-code LangChain-style flows,
  components, agents, retrieval, and app prototyping.
- [Dify](https://github.com/langgenius/dify) [![stars](https://img.shields.io/github/stars/langgenius/dify?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langgenius/dify) [![commits](https://img.shields.io/github/commit-activity/m/langgenius/dify?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langgenius/dify): Type:
  `daemon`.
  self-hosted LLM app platform. Builds chatbots, workflows, agents, knowledge
  apps, and API-backed AI products with a managed UI.

[Back to top](#awesome-ai)

## Sandboxes, Guardrails, And Policy

- [Daytona](https://github.com/daytonaio/daytona) [![stars](https://img.shields.io/github/stars/daytonaio/daytona?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/daytonaio/daytona) [![commits](https://img.shields.io/github/commit-activity/m/daytonaio/daytona?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/daytonaio/daytona):
  `daemon` `sdk`.
  Type: secure development environment and workspace runtime. Strong candidate
  for isolating AI-generated code execution and disposable agent workspaces.
- [E2B](https://github.com/e2b-dev/E2B) [![stars](https://img.shields.io/github/stars/e2b-dev/E2B?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/e2b-dev/E2B) [![commits](https://img.shields.io/github/commit-activity/m/e2b-dev/E2B?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/e2b-dev/E2B):
  `daemon` `sdk`.
  Type: sandbox runtime for AI agents and generated code. Useful for hosted or
  ephemeral execution where agents need an isolated compute environment.
- [HumanLayer](https://github.com/humanlayer/humanlayer) [![stars](https://img.shields.io/github/stars/humanlayer/humanlayer?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/humanlayer/humanlayer) [![commits](https://img.shields.io/github/commit-activity/m/humanlayer/humanlayer?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/humanlayer/humanlayer):
  `daemon`.
  Type: human-in-the-loop approval layer for agents. Useful for coding and ops
  agents that need explicit human approval before contacting people, changing
  external systems, deploying, or touching sensitive resources.
- [NeMo Guardrails](https://github.com/NVIDIA-NeMo/Guardrails) [![stars](https://img.shields.io/github/stars/NVIDIA-NeMo/Guardrails?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/NVIDIA-NeMo/Guardrails) [![commits](https://img.shields.io/github/commit-activity/m/NVIDIA-NeMo/Guardrails?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/NVIDIA-NeMo/Guardrails):
  `plugin` `sdk` `daemon`.
  Type: conversational guardrails framework. Provides policy and behavior
  controls for production LLM applications and assistant workflows.
- [Guardrails AI](https://github.com/guardrails-ai/guardrails) [![stars](https://img.shields.io/github/stars/guardrails-ai/guardrails?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/guardrails-ai/guardrails) [![commits](https://img.shields.io/github/commit-activity/m/guardrails-ai/guardrails?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/guardrails-ai/guardrails):
  `sdk` `daemon`.
  Type: validation and schema guardrails framework. Helps constrain,
  validate, and repair model outputs before application code trusts them.
- [Open Policy Agent (OPA)](https://github.com/open-policy-agent/opa) [![stars](https://img.shields.io/github/stars/open-policy-agent/opa?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/open-policy-agent/opa) [![commits](https://img.shields.io/github/commit-activity/m/open-policy-agent/opa?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/open-policy-agent/opa):
  `cli` `daemon`.
  Type: general policy engine. Useful as a real authorization and policy
  boundary for agent tools, deployment actions, secrets, and infrastructure
  workflows.

[Back to top](#awesome-ai)

## Evaluation, Observability, And Model Routing

- [LiteLLM](https://github.com/BerriAI/litellm) [![stars](https://img.shields.io/github/stars/BerriAI/litellm?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/BerriAI/litellm) [![commits](https://img.shields.io/github/commit-activity/m/BerriAI/litellm?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/BerriAI/litellm): Type: LLM API gateway and
  `daemon` `plugin` `sdk`.
  model router. Provides provider/base-url routing and shared API gateway
  behavior. Token/cost note: centralizes routing, budgets, and model selection
  when multiple providers are actually needed.
- [DSPy](https://github.com/stanfordnlp/dspy) [![stars](https://img.shields.io/github/stars/stanfordnlp/dspy?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/stanfordnlp/dspy) [![commits](https://img.shields.io/github/commit-activity/m/stanfordnlp/dspy?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/stanfordnlp/dspy): Type:
  `sdk` `daemon`.
  LLM programming and optimization framework. Defines modular LM programs and
  optimizes prompts, demonstrations, and pipelines against evaluation signals.
- [FreeLLMAPI](https://github.com/tashfeenahmed/freellmapi) [![stars](https://img.shields.io/github/stars/tashfeenahmed/freellmapi?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/tashfeenahmed/freellmapi) [![commits](https://img.shields.io/github/commit-activity/m/tashfeenahmed/freellmapi?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/tashfeenahmed/freellmapi): Type:
  `daemon` `plugin` `sdk`.
  OpenAI-compatible LLM API proxy and router. Aggregates multiple free-tier or
  custom OpenAI-compatible endpoints behind one `/v1` surface. Safety note:
  review provider terms, key handling, and routing behavior before use.
- [Langfuse](https://github.com/langfuse/langfuse) [![stars](https://img.shields.io/github/stars/langfuse/langfuse?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/langfuse/langfuse) [![commits](https://img.shields.io/github/commit-activity/m/langfuse/langfuse?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/langfuse/langfuse): Type: LLM observability and
  `daemon` `sdk`.
  tracing platform. Tracks prompts, generations, traces, evaluations, and
  datasets for API-backed AI apps.
- [Helicone](https://github.com/Helicone/helicone) [![stars](https://img.shields.io/github/stars/Helicone/helicone?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Helicone/helicone) [![commits](https://img.shields.io/github/commit-activity/m/Helicone/helicone?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Helicone/helicone): Type: LLM observability and
  `daemon` `plugin` `sdk`.
  gateway/proxy platform. Tracks requests, latency, cost, feedback, caching,
  and provider behavior.
- [OpenLLMetry](https://github.com/traceloop/openllmetry) [![stars](https://img.shields.io/github/stars/traceloop/openllmetry?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/traceloop/openllmetry) [![commits](https://img.shields.io/github/commit-activity/m/traceloop/openllmetry?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/traceloop/openllmetry): Type:
  `plugin` `daemon` `sdk`.
  OpenTelemetry instrumentation for LLM applications. Memory type: event-log
  and tool-output evidence for traces, prompts, completions, and tool calls;
  retention and redaction need review before broad capture.
- [Phoenix](https://github.com/Arize-ai/phoenix) [![stars](https://img.shields.io/github/stars/Arize-ai/phoenix?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/Arize-ai/phoenix) [![commits](https://img.shields.io/github/commit-activity/m/Arize-ai/phoenix?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/Arize-ai/phoenix): Type:
  `plugin` `daemon` `sdk`.
  AI observability and evaluation platform. Provides tracing, experiments,
  evals, datasets, prompt analysis, and LLM application debugging workflows.
- [promptfoo](https://github.com/promptfoo/promptfoo) [![stars](https://img.shields.io/github/stars/promptfoo/promptfoo?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/promptfoo/promptfoo) [![commits](https://img.shields.io/github/commit-activity/m/promptfoo/promptfoo?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/promptfoo/promptfoo): Type:
  `plugin` `sdk` `daemon`.
  prompt and model regression testing framework. Runs test matrices across
  prompts, providers, assertions, red-team checks, and CI workflows.
- [Argilla](https://github.com/argilla-io/argilla) [![stars](https://img.shields.io/github/stars/argilla-io/argilla?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/argilla-io/argilla) [![commits](https://img.shields.io/github/commit-activity/m/argilla-io/argilla?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/argilla-io/argilla):
  `sdk` `daemon`.
  Type: data feedback and labeling platform. Useful for building eval
  datasets, human feedback loops, preference data, and review queues for LLM
  and voice-agent systems.
- [autoevals](https://github.com/braintrustdata/autoevals) [![stars](https://img.shields.io/github/stars/braintrustdata/autoevals?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/braintrustdata/autoevals) [![commits](https://img.shields.io/github/commit-activity/m/braintrustdata/autoevals?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/braintrustdata/autoevals):
  `plugin` `sdk` `daemon`.
  Type: evaluation library from the Braintrust ecosystem. Provides reusable
  LLM eval scorers and utilities; represent Braintrust SaaS/SDK separately and
  review hosting, retention, and licensing before adopting broadly.
- [DeepEval](https://github.com/confident-ai/deepeval) [![stars](https://img.shields.io/github/stars/confident-ai/deepeval?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/confident-ai/deepeval) [![commits](https://img.shields.io/github/commit-activity/m/confident-ai/deepeval?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/confident-ai/deepeval): Type:
  `plugin` `sdk` `daemon`.
  LLM evaluation framework. Provides unit-test-like evals, metrics, datasets,
  benchmarks, and CI-friendly checks for LLM applications.
- [Ragas](https://github.com/vibrantlabsai/ragas) [![stars](https://img.shields.io/github/stars/vibrantlabsai/ragas?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/vibrantlabsai/ragas) [![commits](https://img.shields.io/github/commit-activity/m/vibrantlabsai/ragas?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/vibrantlabsai/ragas): Type:
  `sdk` `lib`.
  RAG evaluation framework. Measures retrieval, generation, faithfulness,
  context relevance, answer quality, and related RAG-specific metrics.
- [llmfit](https://github.com/AlexsJones/llmfit) [![stars](https://img.shields.io/github/stars/AlexsJones/llmfit?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/AlexsJones/llmfit) [![commits](https://img.shields.io/github/commit-activity/m/AlexsJones/llmfit?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/AlexsJones/llmfit): Type: LLM fit/evaluation
  `daemon` `sdk`.
  tooling. Tracked for future evaluation workflows.

[Back to top](#awesome-ai)

## Non-Source Utilities

- [Obsidian CLI](https://obsidian.md/cli): Type: official CLI for Obsidian
  `cli` `daemon` `lib`.
  Markdown vaults. Useful for agent-assisted note, doc, and knowledge-work
  workflows over local `.md` files. Memory type: filesystem/Markdown vault
  memory, not vector/RAG memory by itself. Source note: Obsidian is proprietary
  and this is included as an explicit non-source exception.

[Back to top](#awesome-ai)

## Reference Lists And Research

- [AI Engineering from Scratch](https://github.com/patchy631/ai-engineering-hub) [![stars](https://img.shields.io/github/stars/patchy631/ai-engineering-hub?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/patchy631/ai-engineering-hub) [![commits](https://img.shields.io/github/commit-activity/m/patchy631/ai-engineering-hub?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/patchy631/ai-engineering-hub):
  `daemon` `lib`.
  Type: learning/reference repository. Useful for AI engineering examples and
  learning material, not a runtime stack component.
- [Hamel evals](https://github.com/hamelsmu/hamel) [![stars](https://img.shields.io/github/stars/hamelsmu/hamel?style=flat&color=gold&label=stars%2Fmonth)](https://github.com/hamelsmu/hamel) [![commits](https://img.shields.io/github/commit-activity/m/hamelsmu/hamel?style=flat&color=blue&label=commits%2Fmonth)](https://github.com/hamelsmu/hamel): Type: evaluation guidance
  `sdk` `lib`.
  and examples repository. Useful for practical eval setup notes.
- [Glama MCP Registry](https://glama.ai/mcp/servers): Type: MCP registry and
  `daemon` `mcp` `lib`.
  discovery service. Useful for finding popular MCP servers by category and
  stars.
- [PulseMCP](https://www.pulsemcp.com/): Type: MCP registry and news/discovery
  `daemon` `mcp` `lib`.
  service. Useful for tracking current MCP tools and ecosystem activity.
- [aitmpl](https://aitmpl.com/): Type: AI coding template and tool directory.
  `mcp` `skill` `daemon` `lib`.
  Useful for discovering Claude Code templates, agents, commands, skills, and
  MCP integrations.
