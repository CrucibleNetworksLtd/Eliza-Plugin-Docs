---
title: MessageAgent
layout: default
---

![](MessageAgent.png)

Sends a message to an agent.

# Inputs

| - | - | - |
|Type|Name|Description|
|FString|AgentId|The ID string of the agent to send the message to.|
|FString|Message|The message to send to the agent.|

# Outputs

| - | - | - |
|Type|Name|Description|
|bool|Success|If this method was a HTTP success, usable as a quick check to see if it immediately failed.|
|FString|User||
|FString|Text|The text returned by the Eliza AI, usually representing what the AI is saying in response to what you sent as a message.|
|FString|Action|Any actions the AI tried to perform.|

# C++
Module: `Eliza`
include: `#include "MessageAgent.h"`

`UMessageAgent::MessageAgent()` - instantiates this async method.
`Activate()` - Activates this async method.
In C++, the outputs of the async function can be acted upon by binding to the event delegate "`OnMessageAgentCompleted`".
