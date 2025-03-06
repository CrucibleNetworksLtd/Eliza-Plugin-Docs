---
title: CreateNewCharacter
layout: default
parent: Home
---

![](CreateNewCharacter.png)

Creates a new Eliza agent on the server with the given character. The GUID of the agent is returned as AgentID.

# Inputs

| - | - | - |
|Type|Name|Description|
|FAgentDetailsCharacter|AgentCharacter|The character struct that the agent will use.|
|UElizaInstance\*|ElizaInstance|The Eliza instance that we should be communicating with. This can either be a ElizaInstance game asset created in the content browser, or created on the fly with the CreateElizaInstance method.|

# Outputs

| - | - | - |
|Type|Name|Description|
|bool|Success|If this method was a HTTP success, usable as a quick check to see if it immediately failed.|
|FString|AgentID|The AgentID of the newly created Agent.|

# C++
Module: `Eliza`
include: `#include "CreateNewCharacter.h"`

`UCreateNewCharacter::CreateNewCharacter(FAgentDetailsCharacter AgentCharacter, UElizaInstance* ElizaInstance)` - instantiates this async method.
`Activate()` - Activates this async method.
In C++, the outputs of the async function can be acted upon by binding to the event delegate "`OnCreateNewCharacterCompleted`".
