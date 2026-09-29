---
title: "Pokedex REPL"
summary: "Interactive Go REPL for exploring the PokéAPI, with a custom time-based response cache."
tags: ["Go", "REST API", "Caching"]
repo: "https://github.com/cm-brown/pokedex"
weight: 4
---
A command-line REPL in Go for exploring Pokémon locations and catching and inspecting Pokémon through the PokéAPI.

**What I focused on:** a separate API client package, and a thread-safe in-memory cache with a reap loop that expires entries, so repeated requests are instant.
