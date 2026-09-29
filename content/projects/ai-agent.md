---
title: "AI Coding Agent"
summary: "Python agent that uses Gemini function calling to list, read, write, and run files in a sandboxed directory."
tags: ["Python", "LLM", "Function calling"]
repo: "https://github.com/cm-brown/ai-agent"
weight: 2
---
A small command-line agent in the style of an AI coding assistant. You give it a task, and it loops: Gemini decides which tool to call, and the program runs that tool and returns the result to the model until the task is done.

**Tools the model can call:** list files, read file contents, write files, and run Python files. All of them are restricted to a working directory.

I built it to learn how agent loops and tool schemas actually work under the hood.
