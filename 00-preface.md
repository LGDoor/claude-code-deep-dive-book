# Preface

## Claude Code in one paragraph

Claude Code is a terminal-first coding assistant, but the most useful way to understand it is as a session-oriented orchestration runtime. It captures user intent, builds model-facing context, exposes governed tools, persists durable sessions, and extends outward through integrations, background work, and multi-agent coordination. This book studies that architecture rather than teaching the day-to-day command surface.

## Who this book is for

Claude Code Deep Dive is written for readers who need a system-level mental model before they work on or around the product:

- contributors who want to understand the runtime before changing it
- integrators who need to place plugins, MCP servers, skills, LSP, or remote surfaces in the larger design
- architects and operators who care about how an agentic coding system stays durable, extensible, and policy-aware

The book assumes familiarity with terminal workflows, source control, and the general idea of language-model tool use. It does **not** assume prior knowledge of Claude Code's internal structure.

## What this book is and is not

This is not a user manual, a prompt cookbook, or a line-by-line code tour. It does not try to document every command, every feature flag, or every minor helper. Instead, it asks a narrower question: **what architectural ideas make Claude Code behave the way it does?**

That focus shapes the whole manuscript. The chapters spend their time on execution models, context construction, policy boundaries, persistence, extension layers, and operational tradeoffs rather than on enumerating surface features.

## How this book relates to the implementation

The discussion is grounded in the current `src/` implementation. File paths appear throughout the chapters as anchors, but the narrative stays at the level of subsystems, control flow, contracts, and design tradeoffs. The goal is to explain why the implementation is shaped the way it is, not to paraphrase individual source files.

## How to read the rest of the book

Chapter 1 introduces the vocabulary and overall mental model, including the glossary that later chapters rely on. Chapters 2 through 5 explain the runtime core: turn execution, context construction, tools, and policy. Chapters 6 through 8 explain how Claude Code is surfaced and extended. Chapters 9 through 11 explain how Claude Code survives over time: persistence, multi-agent coordination, and operational shape. Chapter 12 closes by restating the design thesis that connects those parts into one system.
