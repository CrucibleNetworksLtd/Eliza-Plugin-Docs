---
title: Home
layout: home
---

The Eliza Plugin provides simple BP and C++ APIs for integrating the Eliza autonomous agent framework into Unreal Engine, enabling developers to leverage the capabilities of autonomous AI agents, enhancing gameplay experiences with dynamic AI interactions.
Easy-to-use Blueprint async nodes and C++ events for Eliza for API communications with the Eliza Framework:
* MessageAgent - Allows you to send messages to an agent running in your Eliza instance, returns the next message, and any actions data if it is present.
* GetAgents - Returns an array of all the agents running in your Eliza instance.
* GetAgentCharacter - Given an AgentId, returns details about a the character that agent is representing from its character file.

We are planning to add more features from Eliza v1, and to support Eliza v2 as it becomes available.

# Getting Started
Please note that this plugin doesn't run an Eliza for you, but instead talks to an existing Eliza instance. You must have a running instance of accessible over HTTP either locally or on a server. You can learn how to set up Eliza with the [Eliza docs](https://elizaos.github.io/eliza/docs/intro/), or by [watching the excelent video tutorial series by Shaw](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL). Make sure you have that working first before trying to use this plugin.

All of the functionality of this plugin is accessable via both Blueprints "Async Actions" and C++. 

The following pages document each async action:

## MessageAgent

## GetAgents

## GetAgentCharacter
